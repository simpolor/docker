# 도커 버전 확인
```
> docker --version
> docker -v
```

# 도커 이미지 검색
```
> docker search {이미지명}
> docker search mysql
> docker search redis
```

# 도커 이미지 다운로드
```
> docker pull {이미지명}
> docker pull mysql:lastest ( #mysql 마지막 버전 다운로드 )
```

# 도커 이미지 확인
```
> docker images
> docker image ls
```

# 도커 프로세스 확인
```
> docker ps
> docker ps -a
```

# 컨테이너 간 통신 시 localhost로 접근
# 만약 하지 않을 경우 IP 주소로 접근해야함
> docker network create backend-network