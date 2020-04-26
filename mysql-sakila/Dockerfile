FROM mysql:8

RUN apt-get update && \
apt-get install -y wget &&\
wget https://downloads.mysql.com/docs/sakila-db.tar.gz && \
tar -xzf sakila-db.tar.gz && \
cp ./sakila-db/sakila-schema.sql /docker-entrypoint-initdb.d/1-sakila-schema.sql && \
cp ./sakila-db/sakila-data.sql /docker-entrypoint-initdb.d/2-sakila-data.sql


