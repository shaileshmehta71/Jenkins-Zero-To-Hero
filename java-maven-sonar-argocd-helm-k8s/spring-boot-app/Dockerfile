# Java 11, multi-arch (arm64/amd64)
FROM eclipse-temurin:11-jre-jammy

# Path to your built JAR (adjust if needed)
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app
COPY ${artifact} app.jar

# Optional JVM flags via env
ENV JAVA_OPTS=""

ENTRYPOINT ["sh","-c","java $JAVA_OPTS -jar app.jar"]
