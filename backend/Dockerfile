FROM openjdk:12-alpine
VOLUME /tmp
COPY /target/shop-api-0.0.1-SNAPSHOT.jar shop-api-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java", "-jar","shop-api-0.0.1-SNAPSHOT.jar", "--spring.profiles.active=docker"]
