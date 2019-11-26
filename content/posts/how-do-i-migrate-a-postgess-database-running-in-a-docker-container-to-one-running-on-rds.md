+++
title = "How do I migrate a postgess database running in a docker container to one running on RDS?"
author = ["T", "Ivan"]
lastmod = 2019-11-26T17:24:03+09:00
weight = 2005
draft = false
+++

## How do I set up a PG DB on RDS. {#how-do-i-set-up-a-pg-db-on-rds-dot}

first what do I need? well in this case this is a POC[^fn:1] project, not a real build. So I don't need to think too
much about provisioning anything with sensible amounts of
resource. I will make the assumption that there is some resource
configuration that will match our apps needs, but I don't want to
figure that out for now. I want to just make some thing quick and
cheap. why not a t3.micro with none of the features enabled..
So I guess I need a PG instance of the same version as our docker
db.


### Links {#links}

-   <https://dev.to/jamby1100/deploy-rails-in-amazon-ecs-part-3-create-the-rds-database-task-definition-and-load-balancer-1ffe>


## How do i migrate data from docker to RDS {#how-do-i-migrate-data-from-docker-to-rds}

Transition to AWS RDS:

-   Login to your machine.
    -   Stop the application docker- docker stop <application\_docker\_name>
    -   Check the website - should be down
-   Login to postgres container- docker exec -it <postgres\_docker\_name> bash
    -   Take a dump of your database:
        -   pg\_dump -Fc -v -h localhost -U <username> -d <db\_name> -p 5432 > dump\_file.dump
    -   Copy the database to AWS RDS:While you’re in your postgres container:
        -   pg\_restore -c -h <aws\_rds\_link> -U <username> -d <db\_name> -v dump\_file.dump
-   Login to AWS RDS, validate the last entries in some tables.
-   Deploy the new code (with the new AWS RDS url)
-   Check your website - should be up and running
-   Validate some db updates
-   Stop the postgres container and remove it.
-   Most important step, first try it in your dev environment or staging before moving to productionAH


### Links {#links}

-   <https://medium.com/@aditya_misra5/move-your-local-postgres-db-container-to-rds-in-12-simple-steps-84f9fd450c9e>


## What might the change path look like for production? {#what-might-the-change-path-look-like-for-production}

1.  Clone  production all up to speed with the current build on the
    docker container. and make sure it's okay.
2.  make an outage period where we take a dump of the docker-db and load
    it to RDS-db
3.  update production to use RDS endpoints for db. start it up and
    test it out.
    -   point it back at the docker instance if its not working.
4.  Bonus points ..
    -   clone prod to a staging environment .. and do it
        once there first
    -   How can you make sure users dont lose data if they input it
        into the new system and something goes wrong?

[^fn:1]: proof of concept
