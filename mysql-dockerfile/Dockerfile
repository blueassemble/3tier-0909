FROM mysql:8.0.26

RUN apt-get -y update && apt-get -y upgrade

COPY ./utf8.cnf /etc/mysql/conf.d/

ENV MYSQL_ROOT_PASSWORD="qwer1234"
#ENV MYSQL_DATABASE="blue"

COPY ./dump-0902.sql /docker-entrypoint-initdb.d/



EXPOSE 3306

