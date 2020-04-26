FROM python:2.7.10

WORKDIR /root

RUN pip install --upgrade pip
RUN pip install setuptools -U
RUN pip install SQLAlchemy==1.3.16 py2neo unicodecsv mysql-connector
RUN mkdir /config

COPY pysql2neo4j /root/pysql2neo4j
RUN rm /root/pysql2neo4j/settings.ini && ln -s /config/settings.ini /root/pysql2neo4j/settings.ini

VOLUME /config
