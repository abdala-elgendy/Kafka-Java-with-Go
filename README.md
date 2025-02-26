it is a small implementation to apply Kafka and producer-consumer pattern with Java and Golang throughout Kafka 

## How to run the project 

run docker 
```sh
docker-compose up
```
go into Kafka and determine the partitions and replication factor 
```sh
docker exec -it kafka /bin/bash
kafka-topics.sh --create --topic=fancy-topic --partitions=1 --replication-factor=1 --zookeeper=zookeeper:2181
```
run producer ( producer.go) and consumer (app.java)

```sh
go run producer.go
```
