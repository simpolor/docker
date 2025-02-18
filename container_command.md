# 도커 컨테이너 목록 확인
```
> docker container ls
```

# 도커 컨테이너 종료
> docker stop {컨테이너ID}

# 도커 컨테이너 실행
> docker start <컨테이너ID>

# 도커 새로운 컨테이너 실행
```
> docker run <옵션> <이미지이름 or 이미지ID> <실행할 파일>
> docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=password --name local-mysql -v /Users/simpolor/docker/mysql:/var/lib/mysql mysql:8.0.17 --character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci
``` 

# 도커 docker-compose 파일로 컨테이너 실행
```
> docker-compose up -d
```



# 도커 컨테이너 쉘 접속
```
> docker exec -it {컨테이너 이름} bash
> docker exec -it {컨테이너ID} /bin/bash
> docker exec -it docker-mysql bash
> docker exec -it docker-mysql /bin/sh
```



