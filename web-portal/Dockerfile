# Base Alpine Linux based image with OpenJDK JRE only

FROM openjdk:8-jre-alpine

# copy application WAR (with libraries inside)
COPY build/libs/sample-web-portal-0.0.1.jar /web-portal.jar

# specify default command
CMD ["/usr/bin/java", "-jar", "-Dspring.profiles.active=test", "/web-portal.jar"]