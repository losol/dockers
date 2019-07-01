# dockers and dockercomposers

## Updating on Docker Hub


```bash
docker build -t mongo-spark-r4 .
docker tag mongo-spark-r4 losolio/mongo-spark-r4
docker login
docker push losolio/mongo-spark-r4
```