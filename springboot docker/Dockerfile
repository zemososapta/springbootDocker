FROM openjdk:8-jdk-alpine
VOLUME /tmp
ADD data-generator-0.0.1-SNAPSHOT.jar app.jar
COPY HL7s /HL7s/
EXPORT 9661
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
