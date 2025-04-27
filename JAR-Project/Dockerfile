FROM openjdk:17-alpine
WORKDIR /app
COPY target/JAR-Project-0.0.1-SNAPSHOT.jar JAR-api.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "JAR-api.jar"]