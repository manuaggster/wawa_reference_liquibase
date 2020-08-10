# Start with a base image containing Java runtime
FROM adoptopenjdk/openjdk11

# Create work folder
RUN mkdir /work

# Set environment variable
ENV SECRETSVOL $SECRETSVOL

# Make port 8102 available to the world outside this container
EXPOSE 8102

# Copying the application's jar file inside the container
COPY app/target/app-1.0-SNAPSHOT.jar /work/app.jar

# Run the jar file 
CMD java -jar /work/app.jar