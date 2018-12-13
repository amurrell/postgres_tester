# POSTGRESQL TESTER

```
docker pull postgres
mkdir -p $HOME/docker/volumes/postgres # creates directory for your data to persist via attached volume
```

then start it up,

```
./postgres-up
```

or, if you are using proxylocal for network (with DockerLocal containers) do

```
./postgres-up-proxylocal
```

## Connect from your host machine using:

- host: 0.0.0.0
- user: postgres
- pass: docker
- port: 5432
- db: postgres

## Connect from a DockerLocal container (w/ ProxyLocal)

- host: pg-docker
- user: postgres
- pass: docker
- port: 5432
- db: postgres


## Data

Persists via `$HOME/docker/volumes/postgres` attached volume