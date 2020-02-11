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