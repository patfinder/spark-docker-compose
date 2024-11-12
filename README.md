
- Source: [Testing Apache Spark locally: docker-compose and Kubernetes deployment.](https://shorturl.at/utuyc)

- Create Dockerfile file
- Create start-spark.sh file used by container

- Build docker image

```shell
docker build -t our-own-apache-spark:3.4.0 .
```

- Create docker-compose.yml file
- Run Spark with docker-compose

```shell
docker-compose up
```

- Check running containers (master and 2 workers)

```shell
docker ps
```

- Open Spark web UI: http://localhost:9090/

```shell
docker exec -i -t spark-docker-compose-spark-master-1 /bin/bash

cd /bin
/opt/spark/bin/spark-submit --master spark://0.0.0.0:7077 --name spark-pi --class org.apache.spark.examples.SparkPi  local:///opt/spark/examples/jars/spark-examples_2.12-3.4.0.jar 100
```


```shell


```

```shell
```

```shell
```

```shell
```

```shell
```


