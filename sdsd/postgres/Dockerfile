FROM postgres:11.3-alpine

# works only on fresh db, if volume already contains data, will not run
COPY ./enable_extensions.sql /docker-entrypoint-initdb.d/

ENV POSTGRES_USER=dmytro \
    POSTGRES_PASSWORD=password\
    POSTGRES_DB=books