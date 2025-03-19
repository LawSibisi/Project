
FROM openjdk:17-jdk-slim

WORKDIR /app

COPY . /app

RUN apt-get update && apt-get install -y maven

RUN mvn clean package

ENTRYPOINT ["java", "-jar", "/target/WeBuyBusiness-Sinethemba-1.0-SNAPSHOT.jar"]


EXPOSE 8080

