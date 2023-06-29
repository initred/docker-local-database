# Docker Local Database

A repository for fast database execution with dockers in a local development environment.

## Support Database

- [MySQL](https://www.mysql.com/) [Default]
- [MariaDB](https://mariadb.org/)
- [Postgres](https://www.postgresql.org/)
- [Redis](https://redis.io/)
- [MongoDB](https://www.mongodb.com/)

## How To Use

```
git clone https://github.com/initred/docker-local-database
```

```
cd docker-local-database
```

Uncomment the required database in "docker-compose.yml".
By default, only MySQL is unannotated.

If you need to set up a database. Modify the ".env" file.

**For your information, mariadb is the same as mysql's environment variable.**

## How To Run

Run all databases used in docker-compose.yml in the background

```shell
docker-compose up -d
```

Run individually in the background of the database used in docker-compose.yml

```shell
docker-compose up -d mysql
```

```shell
docker-compose up -d mariadb
```

```shell
docker-compose up -d pgsql
```

```shell
docker-compose up -d redis
```

```shell
docker-compose up -d mongodb
```

## How To Stop

Stops all databases used in docker-compose.yml.

```shell
docker-compose stop
```

Stops the database used in docker-compose.yml individually.

```shell
docker-compose stop mysql
```

```shell
docker-compose stop mariadb
```

```shell
docker-compose stop pgsql
```

```shell
docker-compose stop redis
```

```shell
docker-compose stop mongodb
```

## How To Down

Drop all databases used in docker-compose.yml.

```shell
docker-compose down
```

**Enjoy it Development!**
