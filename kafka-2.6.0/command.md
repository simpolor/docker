# Zookeeper 및 Kafka Docker 이미지 다운로드
```
> docker pull zookeeper:3.4.14
> docker pull wurstmeister/kafka:2.13-2.6.3
```

# Kafka Docker 이미지 태그 생성
```
> docker tag wurstmeister/kafka:2.13-2.6.3 kafka:2.6.0
```

# Zookeeper 및 Kafka Docker 실행
```
> docker run -d -p 2181:2181 --name zookeeper zookeeper:3.4.14
> docker run -d -p 9092:9092 --name docker-kafka-2.6 -v ~/docker/kafka-2.6.0:/kafka/kafka-logs --link zookeeper -e KAFKA_ZOOKEEPER_CONNECT=zookeeper:2181 -e KAFKA_LISTENERS=PLAINTEXT://0.0.0.0:9092 -e KAFKA_ADVERTISED_LISTENERS=PLAINTEXT://localhost:9092 -e KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR=1 kafka:2.6.0
```