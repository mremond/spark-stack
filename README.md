# spark-stack

## Commands

### Start stack

```
docker-compose up 
```

### Connect to Kafka server

```
docker exec -it $(docker-compose ps -q kafka) bash
```

You can thus use Kafka tool to create topic:

```
kafka-topics --create --zookeeper zookeeper --replication-factor 1 --partitions 2 --topic word-count
```
