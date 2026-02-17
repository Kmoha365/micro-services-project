FROM eclipse-temurin:21-jdk-alpine
WORKDIR /app
COPY target/*.jar name-server.jar
EXPOSE 8761
ENTRYPOINT [ "java","-jar","/app/name-server.jar" ]