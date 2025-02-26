# RabbitMQ Docker 이미지 다운로드
```
> docker pull rabbitmq:3.13.7-management
```

# RabbitMQ Docker 이미지 태그 생성
```
> docker tag rabbitmq:3.13.7-management rabbitmq:3.13.7
```

# RabbitMQ Docker 실행
```
docker run -d -p 15672:15672 -p 5672:5672 -e 'RABBITMQ_DEFAULT_USER=admin' -e 'RABBITMQ_DEFAULT_PASS=admin' --name docker-rabbitmq-3.13.7 -v ~/docker/rabbitmq-3.13.7:/var/lib/rabbitmq rabbitmq:3.13.7
```