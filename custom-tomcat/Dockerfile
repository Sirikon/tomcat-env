FROM tomcat:8.5-jre8

RUN apt-get update && apt-get install -y nano vim

COPY manager.xml /usr/local/tomcat/conf/Catalina/localhost/manager.xml
COPY tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
COPY web.xml /usr/local/tomcat/webapps/manager/WEB-INF/web.xml
