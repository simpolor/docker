# MongoDB Docker 이미지 다운로드
```
> docker pull mongo:7.0
```

# MongoDB Docker 실행
```
> docker run -d -p 27017:27017 --name docker-mongodb-7.0 -v ~/docker/mongodb-7.0:/data/db -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=pass1234 mongo:7.0
```
