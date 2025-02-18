# Elasticsearch Docker 이미지 다운로드
```
> docker pull docker.elastic.co/elasticsearch/elasticsearch:7.6.2
```

# Redis Docker 실행
```
> docker run -d -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.6.2 -v ~/docker/mysql:/usr/share/elasticsearch/data
```