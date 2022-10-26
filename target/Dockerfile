
FROM ubuntu:jammy

RUN mkdir /opt/app

RUN apt-get update

RUN apt install openjdk-11-jdk -y

WORKDIR /opt/app 

ADD ./example.smallest-0.0.1-SNAPSHOT.jar /opt/app/example.jar

EXPOSE 8080

RUN ["chmod", "+x", "/opt/app/example.jar"] 

ENTRYPOINT ["java" , "-jar" , "example.jar"]
