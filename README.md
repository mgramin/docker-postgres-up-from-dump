# docker-postgres-up-from-dump


## Build it:


Build with Postgres Pro demo database dump:
```
docker build --build-arg DUMP_URI=https://edu.postgrespro.ru/demo-small.zip -t postgres-pro-small-demo-db .
```

Build without dump:
```
docker build --build-arg .
```


## Run it:

```
docker run -d --name pg_demo_db -e POSTGRES_PASSWORD=postgres -t -p 5432:5432 postgres-pro-small-demo-db
```
