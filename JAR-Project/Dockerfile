FROM openjdk:17-jdk-slim
RUN rm -rf /usr/local/tomcat/webapps/*
RUN apt-get update && apt-get upgrade -y && apt-get clean
WORKDIR /app
COPY target/JAR-Project-0.0.1-SNAPSHOT.jar JAR-api.jar
EXPOSE 8080
HEALTHCHECK --interval=10s --timeout=3s --retries=3 \
CMD curl --fail http://localhost:8080/ || exit 1
ENTRYPOINT ["java", "-jar", "JAR-api.jar"]
