# Elasticsearch Docker 이미지 다운로드
```
> docker pull docker.elastic.co/elasticsearch/elasticsearch:7.6.2
```

# Elasticsearch Docker 이미지 태그 생성
```
> docker tag docker.elastic.co/elasticsearch/elasticsearch:7.6.2 elasticsearch:7.6.2
```

# Redis Docker 실행
```
> docker run -d -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" -e "cluster.name=docker-cluster" -e "ES_JAVA_OPTS=-Xms512m -Xmx512m" --name docker-elasticsearch-7.6.2 -v ~/docker/elasticsearch-7.6.2:/usr/share/elasticsearch/data docker.elastic.co/elasticsearch/elasticsearch:7.6.2
```