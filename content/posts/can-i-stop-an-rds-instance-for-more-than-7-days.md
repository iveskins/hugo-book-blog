+++
title = "Can I stop an RDS instance for more than 7 days?"
author = ["T", "Ivan"]
lastmod = 2020-03-24T18:20:18+09:00
weight = 2025
draft = false
+++

## Google {#google}

-   <https://cloudiknow.com/rds-stopped-for-more-than-7-days/>
-   <https://github.com/awslabs/aws-instance-scheduler/issues/42>


## Looks like. {#looks-like-dot}

-   can use Cloudwatch scheduled tasks
-   Can use maintenance windows of rds to start and stop and reset
    7day timer?


## Maybe it's better to delete it if its not being used.. {#maybe-it-s-better-to-delete-it-if-its-not-being-used-dot-dot}

and take a snapshot.
that seems to be the design on the system
if we cant do that then we need to increase our capabilities and
knowlege.

-   how to restore
    -   <https://www.youtube.com/watch?v=fxNmMQvOjbA>
-   What is the cost of keeping a snapshot around?
-   What will this mean in a COC defined environemnt
    -   the deletion should problaly be made by a code chagne..
        becuase even if you put back a new db with all the same
        setting
        the ids of the db will have changed, and terraform wouldnt
        recognise the database as the one it made


## Make it {#make-it}


###  {#}

  default     = "cron(0 9 ? \* MON-FRI \*)"
} # stop every weekday at 18:00JST+9

variable "start\_schedule\_expression" {
  description = "Schedule for lambda execution"
  default     = "cron(50 23 ? \* SUN-THU \*)"
} # start every weekday at 08:50JST+9
