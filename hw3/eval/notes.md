## Workflow Summary

1. Download the documents

2. Get the hash id of each document, and append the id into the documents json file(A)

3. Use openai to generate up to 5 similar questions for each document, generate a json file(B) with id and questions

4. Based on B and A, create a list with the format [question, course, id] and write it into pd.df and then output it as csv.


## How to run elasticSearch in codespaces

```
docker run -it \
    --rm \
    --name elasticsearch \
    -p 9200:9200 \
    -p 9300:9300 \
    -e "discovery.type=single-node" \
    -e "xpack.security.enabled=false" \
    -e "ES_JAVA_OPTS=-Xms512m -Xmx512m" \
    docker.elastic.co/elasticsearch/elasticsearch:8.4.3
```

