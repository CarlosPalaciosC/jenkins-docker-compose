FROM postgres:10.4

ENV TZ=America/Lima

RUN apt-get -y update \	
 && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

COPY init.sql /docker-entrypoint-initdb.d/
