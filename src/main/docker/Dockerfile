FROM openjdk:8-jre-alpine

ENV TZ="Asia/Shanghai" HOME="/root" JVM_PARAMS=" " SPRING_PARAMS=" "

WORKDIR ${HOME}

ADD sharding-proxy-facade-1.0-SNAPSHOT.jar ${HOME}/server.jar

EXPOSE 8080

CMD java $JVM_PARAMS -Djava.security.egd=file:/dev/./urandom -jar ${HOME}/server.jar $SPRING_PARAMS