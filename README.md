# cockroachdb
A minimal playground cluster of cockroachdb

## How to run
```
docker-compose up -d
```

### Set up a table and user example
```
docker-compose exec roach1 ./cockroach user set maxroach --insecure
docker-compose exec roach1 ./cockroach sql --insecure
CREATE DATABASE bank;
GRANT ALL ON DATABASE bank TO maxroach;
```
[Build an app](https://www.cockroachlabs.com/docs/stable/build-an-app-with-cockroachdb.html) in your favorite language

## Web UI
At [localhost:8080](http://localhost:8080/)

## How to stop

```
docker-compose stop
```
