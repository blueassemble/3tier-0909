FROM tomcat:9.0

#mysql-connector 설치 및 압축 풀기 
RUN apt-get -y update && apt-get -y upgrade
RUN wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-8.0.26.tar.gz
RUN tar zxvf mysql-connector-java-8.0.26.tar.gz

#mysql-connector => lib 폴더로
RUN cp -a /usr/local/tomcat/mysql-connector-java-8.0.26/mysql-connector-java-8.0.26.jar /usr/local/tomcat/lib/

#index.jsp 넣을 폴더
RUN mkdir /usr/local/tomcat/webapps/ROOT/

#COPY ./index.jsp /usr/local/tomcat/webapps/ROOT/index.jsp

EXPOSE 8080

