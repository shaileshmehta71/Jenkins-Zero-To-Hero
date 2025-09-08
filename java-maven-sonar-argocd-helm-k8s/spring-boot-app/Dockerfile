# Java 11, Alpine, multi-arch (arm64/amd64)
FROM eclipse-temurin:11-jre-alpine

# Path to your built JAR (adjust if needed)
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app
COPY ${artifact} app.jar

# Optional: pass JVM opts at runtime: docker run -e JAVA_OPTS="..."
ENV JAVA_OPTS=""

ENTRYPOINT ["sh","-c","java $JAVA_OPTS -jar app.jar"]
