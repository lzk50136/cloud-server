FROM openjdk:8-jdk-alpine
VOLUME /tmp
COPY sentinel-dashboard.jar /sentinel-dashboard.jar
EXPOSE 8719
EXPOSE 8989
ENTRYPOINT java -Dserver.port=8989 -Dcsp.sentinel.dashboard.server=localhost:8989 -Dproject.name=sentinel -Xms256m -Xmx256m -jar sentinel-dashboard.jar
