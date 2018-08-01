# Prepare container

```
source .env

docker-compose up -d
docker ps
```

## Install packages and postgres extension

```
docker exec -i -t <ID> /bin/bash
```

```
$ apt-get install git make postgresql-server-dev-10
$ git clone https://github.com/gavinwahl/postgres-json-schema.git
$ cd postgres-json-schema
$ make install
$ exit
```

```
psql
```
