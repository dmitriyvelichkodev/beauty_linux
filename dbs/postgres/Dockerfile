FROM postgres:11.3-alpine

ENV POSTGRES_USER=dmytro \
    POSTGRES_PASSWORD=password \
    POSTGRES_DB=bookshelf

# install additional addons for postgres

## in dockerfile we can't specify mount point fromn the host
VOLUME /var/lib/postgresql/data


# 1) Create new image: docker build --tag="dmytro_postgres:dev" .
# 2) Create continer from the new image: docker container create --name dmytro_postgres_dev dmytro_postgres:dev
# 3) Start newely created container: docker container start dmytro_postgres_dev
# 4) Inside container connect to db: psql <POSTGRES_DB> <POSTGRES_USER>