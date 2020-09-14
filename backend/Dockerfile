#FROM maven:latest AS build
#WORKDIR /app
#COPY . /app
#RUN mvn clean package 


#FROM openjdk:12-alpine
#WORKDIR /app2
#COPY --from=build /app/target/shop-api-0.0.1-SNAPSHOT.jar  /app2/shop-api-0.0.1-SNAPSHOT.jar
#ENTRYPOINT ["postgres" "java","-jar","shop-api-0.0.1-SNAPSHOT.jar", "-spring.profiles.active=docker"]





FROM openjdk:12-alpine
WORKDIR /app
COPY /target/shop-api-0.0.1-SNAPSHOT.jar /app/shop-api-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java", "-jar","shop-api-0.0.1-SNAPSHOT.jar", "--spring.profiles.active=docker"]
