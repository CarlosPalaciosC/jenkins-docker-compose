FROM docker.bintray.io/jfrog/artifactory-oss

ENV TZ=America/Lima
USER root
RUN apt-get -y update \
 && ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

COPY conf/db.properties /var/opt/jfrog/artifactory/etc/
#COPY lib/postgresql-42.2.2.jar /opt/jfrog/artifactory/tomcat/lib/
