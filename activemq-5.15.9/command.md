# ActiveMQ Docker 이미지 다운로드
```
> docker pull rmohr/activemq:5.15.9
```

# ActiveMQ Docker 실행
```
> docker run -d -p 61616:61616 -p 8161:8161 -e 'ACTIVEMQ_ADMIN_LOGIN=admin' -e 'ACTIVEMQ_ADMIN_PASSWORD=password' --name docker-activemq-5.15.9 -v ~/docker/activemq-5.15.9:/data/activemq
```