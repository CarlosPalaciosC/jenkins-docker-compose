# jenkins-docker-compose
Despliegue de jenkins y herramientas adicionales con docker-compose para armar un flujo automatizado en un entorno de desarrollo local

```
sudo mkdir -p /opt/tools-devops/Source/docker/build/{jenkins,artifactory}
sudo chown 1000:1000 /opt/tools-devops/Source/docker/build/jenkins
sudo chown 1030:1030 /opt/tools-devops/Source/docker/build/artifactory

docker-compose up -d
docker ps

docker exec -ti jenkins bash -c "cat /var/jenkins_home/secrets/initialAdminPassword"
```# bitbucket-pipelines-examples
