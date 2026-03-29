# Use the same Java version you used to build (Java 17 is safer)
FROM eclipse-temurin:17-jre-alpine

# Use a wildcard to find the jar file regardless of its name
WORKDIR /opt/app

# This replaces the ARG and COPY steps you had
COPY target/*.jar app.jar

# This stays the same
ENTRYPOINT ["java","-jar","app.jar"]