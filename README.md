# spark-stack

## Commands

### Start stack

``` bash
docker-compose up
```

### Connect to Kafka server

``` bash
docker exec -it $(docker-compose ps -q kafka) bash
```

You can thus use Kafka tool to create topic:

``` bash
kafka-topics --create --zookeeper zookeeper --replication-factor 1 --partitions 2 --topic word-count
```

### Connect to Spark server

``` bash
docker exec -it $(docker-compose ps -q spark) bash
```
