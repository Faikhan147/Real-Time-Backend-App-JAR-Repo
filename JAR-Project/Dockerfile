FROM openjdk:17-jdk-slim
RUN apt-get update && apt-get upgrade -y && apt-get clean
WORKDIR /app
COPY target/JAR-Project-0.0.1-SNAPSHOT.jar JAR-api.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "JAR-api.jar"]
