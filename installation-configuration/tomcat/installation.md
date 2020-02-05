/opt/devops-udemy


Baixar apache-tomcat 8.5.16
https://archive.apache.org/dist/tomcat/tomcat-8/v8.5.16/bin/
https://archive.apache.org/dist/tomcat/tomcat-8/v8.5.16/bin/apache-tomcat-8.5.16.zip

mover para /opt/apache-tomcat-8.5.16
Editar o arquivo: conf/tomcat-users.xml

<!-- configuracao usuario -->
<role rolename="tomcat"/>
<role rolename="manager-gui"/>
<role rolename="manager-script"/>
<user username="tomcat" password="tomcat" roles="tomcat"/>
<user username="manager" password="tomcat" roles="tomcat,manager-gui"/>
<user username="jenkins" password="jenkins" roles="manager-script"/>

 (dar permissão de execussão em tudo, "+x") na pasta bin (não precisa ser em tudo, fiz igual só por praticidade)
cd bin
$ bin > sudo chmod +x ./*
$ bin > ./catalina.sh start
$ bin > tail ../logs/catalina.out

http://localhost:8080/

manager app
user: manager
pass: tomcat
