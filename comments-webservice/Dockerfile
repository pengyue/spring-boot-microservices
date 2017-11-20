# Base Alpine Linux based image with OpenJDK JRE only

FROM openjdk:8-jre-alpine

# copy application WAR (with libraries inside)
COPY build/libs/sample-comments-webservice-0.0.1.jar /comment-service.jar

# specify default command
CMD ["/usr/bin/java", "-jar", "-Dspring.profiles.active=test", "/comment-service.jar"]