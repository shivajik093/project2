FROM centos
RUN yum update -y
RUN yum install java-1.8* -y
RUN yum install wget -y
RUN wget https://mirrors.estointernet.in/apache/tomcat/tomcat-9/v9.0.45/bin/apache-tomcat-9.0.45.tar.gz
RUN tar -xvzf apache-tomcat-9.0.45.tar.gz
COPY addressbook.war apache-tomcat-9.0.45/webapps
CMD apache-tomcat-9.0.45/bin/./catalina.sh run && apache-tomcat-9.0.45/bin/./startup.sh
EXPOSE 8080
