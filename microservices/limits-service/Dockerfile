FROM maven:3.9.9-eclipse-temurin-21 AS builder
WORKDIR /builder
COPY . .
RUN mvn clean package -DskipTests


FROM eclipse-temurin:21-jre-alpine
WORKDIR /app
COPY --from=builder /builder/target/*.jar app.jar
EXPOSE 8000
ENTRYPOINT [ "java","-jar","app.jar" ]

