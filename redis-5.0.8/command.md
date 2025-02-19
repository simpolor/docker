# Redis Docker 이미지 다운로드
```
> docker pull redis:5.0.8
```

# Redis Docker 실행
```
> docker run -d -p 6379:6379 --name docker-redis-5.0.8 -v ~/docker/redis-5.0.8:/data redis:5.0.8 --appendonly yes
```