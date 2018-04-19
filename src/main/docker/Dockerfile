# Start with a base image containing Java runtime
FROM java:8

# Add Maintainer Info
LABEL maintainer="SKP"

# Add a volume pointing to /tmp
VOLUME /tmp


# Add the application's jar to the container
ADD employee-zull-service-0.0.1-SNAPSHOT.jar employee-zull-service.jar

#RUN bash -c 'touch /employee-zull-service.jar'
# Run the jar file 
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/employee-zull-service.jar"]

EXPOSE 8079
