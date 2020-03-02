http://maven.apache.org/
https://archive.apache.org/dist/maven/maven-3/3.5.0/binaries/apache-maven-3.5.0-bin.tar.gz


mova o apache-maven para:
/opt/devops-udemy/apache-maven-3.5.0

criei o .profile_devops na home com o seguinte conteúdo.

PATH="/home/helder/.nvm/versions/node/v12.14.1/bin:/usr/share/Modules/bin:/usr/local/bin:/usr/local/sbin:/usr/bin:/usr/sbin:/home/helder/bin:/var/lib/snapd/snap/bin:/opt/scripts:/opt/android-sdk/tools:/opt/android-sdk/platform-tools:/opt/exercism-linux-64bit/exercism"



# set java
#java -version
export JAVA_HOME="/opt/jdk/jdk1.8.0_72"

# maven settings
#mvn -version
export M2_HOME=/opt/devops-udemy/apache-maven-3.5.0
export M2=$M2_HOME/bin
# export MAVEN_OPTS="-Xms256m -Xmx2048m"
 export PATH=$PATH:$M2%


 # Maven Security Setup
Primeiro olhe o arquivo start-ambient.md para fazer o source o profile devops.

Inicie o JFrog ARtifactory (para gerar os arquivos .xml, já tenho nos arquivos da sessão)
http://localhost:8081
Set Me Up -> libs-resease
Set Me Up -> libs-snapshot

Copie os arquivos .xml da pasta "arquivos-da-sessao" para ~/.m2

Execute o comando
mvn -emp password
copie o hash gerado e coloque na tag "master" do ~/.m2/setting-security.xml

Execute o comando
mvn -ep password
copie o hash gerado e coloque nas tags
servers -> release -> password      <password>{*** Insert password here ***}</password>
servers -> snapshow -> password
do arquivo ~/.m2/settings.xml

Execute o comand
mvn help:describe
vai fazer alguns downloads (vai dar erro no final, não tem problema), vai
aparecer a pasta ~/.m2/repository
