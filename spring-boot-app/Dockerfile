# Use a lightweight base image for Java 11
FROM eclipse-temurin:11-alpine

# Set the working directory inside the container
WORKDIR /opt/app

# Argument for the artifact path
ARG artifact=target/spring-boot-web.jar

# Copy the application JAR file into the container
COPY ${artifact} app.jar

# Expose the default port used by the Spring Boot application
EXPOSE 8080

# Command to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
