FROM eclipse-temurin:21-jdk-alpine

WORKDIR /app

COPY target/*.jar currency.jar

EXPOSE 8081

ENTRYPOINT [ "java","-jar","/app/currency.jar" ]
