# Maven
FROM maven:3-jdk-11
VOLUME /tpm
ADD /target/*.jar app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar"]