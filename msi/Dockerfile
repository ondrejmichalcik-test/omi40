FROM openjdk:11.0.3-jre-slim-stretch
COPY target/*-shaded.jar app.jar
EXPOSE 80
CMD java -Xmx128m -Xms128m -XX:MaxMetaspaceSize=128m -Dmicronaut.server.port=80 -Dmicronaut.config.files=/codenow/config/application.yaml -Dlogback.configurationFile=logback-codenow.xml -jar app.jar
