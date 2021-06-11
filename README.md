# kafka-local

A docker-compose setup to start kafka locally.

## Prerequisites

You have to have docker and docker-compose installed.

## Start Kafka locally

The following command will start kafka in containers. It might take a while
until kafka is ready.

### Start Containers

``` bash
# in the directory of this repository
docker-compose up -d
```

### Check Containers

``` bash
# in the directory of this repository
docker-compose ps
```

## Connect to kafka

There are two options to connect to kafka. One is from your host network and the
other from the internal docker network. Use the host network for debugging and
tinkering around with kafka, but the internal docker network simulates the way
applications would use it.

### Use with kafka-console

Kafka console is installed on every Kafka broker, so you could exec it in the
container:

``` bash
# in the directory of this repository
```

### Use with kafkacat
