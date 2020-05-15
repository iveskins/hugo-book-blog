+++
title = "How can I alarm if my gitlab backups arn't running?"
author = ["T", "Ivan"]
lastmod = 2020-05-15T13:19:11+09:00
weight = 2062
draft = false
+++

I just had an incident where the crontab on my gitlab host had been
removed for about a month. Because of this the backups to s3 had
not been running, and the existing backups were all deleted by the
s3 bucket policy to delete after 14 days. This reveals two problems
with my system. I have a dashboard set up to monitor the bakups,
but no-one looks at it.

-   it is possible to be left with no backups
-   there was no alarming that the backups were not running.


## How can I alarm if the backup didn't run. {#how-can-i-alarm-if-the-backup-didn-t-run-dot}

Seeming as the AWS tools eem to be the most fail safe(unlikely to
have configuration drift), one way
could be to alarm on the items in the s3
bucket. assuming that nothing else but backups should be in this
bucket. I would would idealy want to check each day if a new
backup file has appared, and if not send an alert message.

-   [This](https://stackoverflow.com/questions/59063713/how-to-setup-cloud-watch-alarm-for-s3-bucket-if-no-data-is-received-in-bucket-fo) stackoverflow answer talks about "Create an Amazon
    CloudWatch Events rule to trigger an AWS Lambda function" That
    seems to be a bit complicatione
-   Maybe I can just make the bucket publish to an SNS topic on any
    create event. Then any time a backup runs a notification will
    be published to that topic. We don't care to know if the back up runs
    successfully, that would be information overload. So we can use
    Cloudwatch metrics to set up an alarm to monitor the numbers of
    messages published to that topic per day. If there isn't a
    message published, then we can assume the bakcup hasn't run and
    we need to investigate.


### How can i make this with terraform? {#how-can-i-make-this-with-terraform}

What are the components?

-   SNS topic to recieve s3 file events
-   [S3 Events configuration](https://www.terraform.io/docs/providers/aws/r/s3_bucket_notification.html)

-   Cloudwatch metic
    -   maybe this is can be created together with the alarm.(maybe
        it doesnt need to be created because we are not using a
        custome metric, and it already exists, and we can just query
        it in the alarm config)
-   [Cloud watch alarm](https://www.terraform.io/docs/providers/aws/r/cloudwatch_metric_alarm.html)
    following
    [This](https://webcache.googleusercontent.com/search?q=cache:pweBgqTEfqQJ:https://underthehood.meltwater.com/blog/2019/01/31/monitoring-your-system-heartbeat-using-cloudwatch/+&cd=1&hl=ja&ct=clnk&gl=jp&client=firefox-b-d) example.
    -   We will set the "period" to "one day(in seconds 86400)" (the frequency of backups)
    -   set "treat\_missing\_data" to "breeching"
        -   so if no data (message) is recieved in a day it will invoke the configured "alarm\_action"
    -
-   SNS topic to recieve alarms(use existing)


#### That was annoying. {#that-was-annoying-dot}

There are some big gotcha with policy permissions to get this
working via terraform.. In the end I have just set it up by hand
for the time being because I have other things to get done.

The alarm:

Threshold
NumberOfMessagesPublished < 1 for 1 datapoints within 1 day
Last change
2020-04-20 07:17:25
ARN
arn:aws:cloudwatch:::alarm:gitlab\_backups\_missing

amespace
AWS/SNS
Metric name
NumberOfMessagesPublished
TopicName
ops-gitlab-backup-metrics-monitor
Statistic
Maximum
Period
1 day

Datapoints to alarm
1 out of 1
Missing data treatment
Treat missing data as bad (breaching threshold)
Percentiles with low samples
evaluate

The bucket notification config:
✓　All object create events
　　send to SNS topic:
ops-gitlab-backup-metrics-monitor

And lots of policies to allow that to happen.
