# ActiveMQ Docker 이미지 다운로드
```
> docker pull redis:5.0.8
```

# ActiveMQ Docker 실행
```
> docker run -d -p 61616:61616 -p 8161:8161 --name docker-activemq -v ~/docker/activemq:/data/activemq -e 'ACTIVEMQ_ADMIN_LOGIN=admin' -e 'ACTIVEMQ_ADMIN_PASSWORD=password'
```