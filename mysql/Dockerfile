FROM mysql:5.7.15

MAINTAINER jarl.andre@gmail.com
LABEL maintainer="jarl.andre@gmail.com"

ENV MYSQL_DATABASE=acs \
    MYSQL_USER=acs \
    MYSQL_PASSWORD=acs \
    MYSQL_RANDOM_ROOT_PASSWORD=true

COPY tables /docker-entrypoint-initdb.d/tables
COPY install.sql /docker-entrypoint-initdb.d

EXPOSE 3306
