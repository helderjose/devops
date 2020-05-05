source no ~/.profile_devops
source ~/.profile_devops

# Jenkins
systemctl start docker
docker container ls -a
docker container start <CONTAINER ID> olhe o id do jenkins (se o conteiner do jenkins não existr use run no lugar do start)
docker container start 65935d56656f
docker container stop 65935d56656f
http://localhost:8090
user: admin
pass: password


# Apache Tomcat
cd /opt/devops-udemy/apache-tomcat-8.5.16/bin && ./catalina.sh start
cd /opt/devops-udemy/apache-tomcat-8.5.16/bin && ./catalina.sh stop
cd /opt/devops-udemy/apache-tomcat-8.5.16/bin && tail ../logs/catalina.out

http://localhost:8080/
Clique em Manager App (para outros user e opções olhar o arquivo installation.md do tomcat)
user: manager
pass: tomcat



# Jfrog
não use o ~/.profile_devops nesse terminal.
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