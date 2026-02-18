FROM eclipse-temurin:21-jdk-alpine
WORKDIR /app
COPY target/*.jar currency-exchange.jar
EXPOSE 8000

ENTRYPOINT [ "java","-jar","/app/currency-exchange.jar" ]