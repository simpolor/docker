# MySQL Docker 이미지 다운로드
```
> docker pull mysql:8.0.17
```

# Mysql Docker 실행
```
> docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=password --name docker-mysql -v ~/docker/mysql:/var/lib/mysql mysql:8.0.17 --character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci
```
