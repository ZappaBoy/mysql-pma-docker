# mysql-pma-docker

## Prerequisites
First of all install [docker](https://docs.docker.com/get-docker/) with `docker-compose`.
Then create a `.env` file starting from `.env.example`

```shell
cp .env.example .env
```
Change the `.env` accordingly to your needs.

## How to start
Simply use `docker-compose` to start the containers.

### Use both `mariadb` (definitely better than `mysql`) and `php-my-admin`
```shell
docker-compose up
```
### Use only `mariadb`
```shell
docker-compose -f docker-compose-mysql.yaml up
```

### Use only `php-my-admin`
```shell
docker-compose -f docker-compose-pma.yaml up
```
