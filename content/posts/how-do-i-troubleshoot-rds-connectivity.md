+++
title = "How do I troubleshoot RDS connectivity?"
author = ["T", "Ivan"]
lastmod = 2019-11-27T16:28:45+09:00
weight = 2006
draft = false
+++

## How do I check access to RDS from my EC2 instance. {#how-do-i-check-access-to-rds-from-my-ec2-instance-dot}

The endpoint address and port of an RDS database can be found from
the RDS console on the "Connectivity & security" page.
To test Connectivity from a host to the DB here are some steps to
follow:

1.  confirm the endpoint dns resolves to the IP of the DB
    -   \`nslookup <endpoint>\`
2.  confirm network connectivity from host to the DB
    -   nc <endpoint> <port>
3.  Try to connect with a database client.
    -   psql -h <endpoint>


## Well that didn't work. What should I check? {#well-that-didn-t-work-dot-what-should-i-check}

1.  Is there something else I should be doing?
2.  Is everything turned on?
    -   For example is the RDS instance in a running state or stopped?
3.  Are there typos anywhere?
4.  Am I using the right tool for the job?
5.  Is everything configured like you thought?
    -   IS the RDS instance in the subnet group you expected?
    -   Do you know how things are configured?
6.  is the configuration correct generally speaking?
    -   Do the subnet ACLS and SG allow for traffic between the the Let's check. I'm sure its an ACL or SG problem.
    -   Are RDS Subnet groups correct?

also [here is the aws support docs](https://aws.amazon.com/premiumsupport/knowledge-center/rds-cannot-connect/). It adds

-   Check DNS resolution with nslook up. \`nslookup rds.endpoint\`
    (usually I would ping the resolved IP to check network
    connectivity. .but I have a feeling RDS hosts have ping responders
    turned off.)
-   Then check with telnet or nc
-   As for troubleshooting the network the docs say
    -   check your VPC SGs allow access from client.
    -   (probably also need to check the clients SG and ACLs allow access
        out as well)
    -


### Extra Commands {#extra-commands}

-   install postgress on AmznLinux: \`sudo amazon-linux-extras install postgresql10\`


### Links {#links}

-   [Digital ocean blog](https://www.digitalocean.com/community/tutorials/how-to-use-netcat-to-establish-and-test-tcp-and-udp-connections-on-a-vps)


## Whats is an RDS subnet group? {#whats-is-an-rds-subnet-group}

I made an RDS database, and then had problems connecting to it. It
turns out it had provisioned with an IP from another old projects
subnet, and that subnet's ACL didn't allow access. Why did my DB use
an interface in this seemingly random subnet? Maybe it was because of
the [RDS Subnet group](https://docs.rightscale.com/cm/dashboard/clouds/aws/rds_subnet_groups.html) configuration for this VPC. I had never heared of
this before so lets take a look.

> An RDS Subnet Group is a collection of subnets that you can use to designate for your RDS database instance in a VPC. The database within your VPC will use the Subnet Group and the preferred Availability Zone to select a subnet and an IP address within that subnet. An Elastic Network Interface will be associated to the database instance with that IP address. Note that each DB Subnet Group should have at least one subnet for every Availability Zone in a given Region.

[^fn:1]


## Conclusion {#conclusion}

When I provisioned our general systems VPC and subnets, I did not
account for the need of a second subnet in another AZ, for the use
of RDS. I need to go back to the team and talk about make a new
subnet.

[^fn:1]: RightScale Docs - <https://docs.rightscale.com/cm/dashboard/clouds/aws/rds_subnet_groups.html>
