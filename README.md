# pysql2neo4j-docker-playground
Dockerised environment to play around with pysql2neo4j

## THIS IS NOT READY YET

**It will just create the docker images, it won't run anything for the moment.**


This is supposed to be a bundle of everything necessary to perform a download'n'go test run of pysql2neo4j.

When you clone the repo and type `docker-compose up -d` it will:
* Create an image of `mysql` with the **Sakila** data set loaded
* Pull neo4j docker image
* build a basic python docker image with `pysql2neo4j` installed in it
* and run automatically `pysql2neo4j` to import *Sakila* database into `neo4j`, **according to your settings.ini** file

