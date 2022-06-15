FROM  openjdk:8-jre

MAINTAINER docker-network

ENV TZ=PRC

VOLUME /home/docker-java

RUN mkdir -p /home/docker-java

WORKDIR /home/docker-java

COPY ./docker-java.jar /home/docker-java/docker-java.jar

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

ENTRYPOINT ["java","-jar","/home/docker-java/docker-java.jar"]