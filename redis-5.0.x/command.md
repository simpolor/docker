# Redis Docker 이미지 다운로드
```
> docker pull redis:5.0.8
> docker network create redis-net
```

# Redis Docker 실행
```
> docker run -d -p 6379:6379 --name docker-redis -v ~/docker/redis:/data redis redis-server --network redis-net --appendonly yes
```