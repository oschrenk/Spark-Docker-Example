# Spark-Docker-Example
An example of using Semantive/Spark Docker image with sbt-docker plugin to create and submit a Spark App.

## Requirements
1. [Docker](https://docs.docker.com/engine/installation/) 1.10.0+ and [docker-compose](https://docs.docker.com/compose/) 1.6.0+
2. [SBT](http://www.scala-sbt.org/)

## Running
1. Create docker image of the sbt-application using

```
sbt docker
```

2. Run whole cluster using ```docker-compose```

```docker-compose up```

Docker-compose will run three images:
- Spark master
- Spark worker
- sbt-application (Spark job)
