FROM tomcat:8.5.16-jre8-alpine


RUN ["apt-get", "update"]
RUN ["apt-get", "-y", "install", "vim"]
RUN ["apt-get", "-y", "install", "nano"]
RUN sed -i 's/port="8080"/port="80"/' /usr/local/tomcat/conf/server.xml

CMD ["catalina.sh", "run"]