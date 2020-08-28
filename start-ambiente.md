# Jenkins
systemctl start docker
docker container ls -a
docker container start <CONTAINER ID> olhe o id do jenkins (se o conteiner do jenkins não existr use run no lugar do start)

container que estou usando para fazer o curso: 61e878e13e79

docker container start 61e878e13e79
docker container stop 61e878e13e79
http://localhost:8090
user: admin
pass: password


# Apache Tomcat
source ~/.profile_devops
cd /opt/devops-udemy/apache-tomcat-8.5.16/bin && ./catalina.sh start
cd /opt/devops-udemy/apache-tomcat-8.5.16/bin && ./catalina.sh stop
cd /opt/devops-udemy/apache-tomcat-8.5.16/bin && tail ../logs/catalina.out

http://localhost:8080/
Clique em Manager App (para outros user e opções olhar o arquivo installation.md do tomcat)
user: manager
pass: tomcat



# Jfrog
source ~/.profile_devops
cd /opt/devops-udemy/artifactory-oss-5.4.5/bin && ./artifactory.sh
ctrl + c para parar
http://localhost:8081
usuário e senha padrão:
admin
password

# Spring Tool Suite
cd /opt/devops-udemy/sprint-tool-suite && ./SpringToolSuite4

# repositório
cd /opt/devops-udemy/github/devops-udemy



obs:
Tudo que eu fizer na .m2 do host tenho que colocar na /opt/jenkins-docker/MEU-CONTAINER/jenkins_home/.m2

Usar o ip do notebook no pom.xml do repositório e na .m2 do /opt/container-jenkins