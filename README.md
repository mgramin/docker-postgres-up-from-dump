# docker-postgres-up-from-dump

## build:

    docker build --build-arg .


    docker build --build-arg DUMP_URI=https://edu.postgrespro.ru/demo_small.zip -t postgres-pro-small-demo-db .


    docker build --build-arg DUMP_URI=https://edu.postgrespro.ru/demo_medium.zip -t postgres-pro-medium-demo-db .


    docker build --build-arg DUMP_URI=https://edu.postgrespro.ru/demo_big.zip -t postgres-pro-big-demo-db .


## run:

    docker run -t -p 5432:5432 postgres-pro-small-demo-db


    docker run -t -p 5432:5432 postgres-pro-medium-demo-db


    docker run -t -p 5432:5432 postgres-pro-big-demo-db


