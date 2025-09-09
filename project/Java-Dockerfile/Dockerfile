# Use OpenJDK 17 as base
FROM openjdk:17

# Set working directory
WORKDIR /usr/src/app/

# Copy the Java source file
COPY Hello.java .

# Compile the Java program
RUN javac Hello.java

# Run the Java program
CMD ["java", "Hello"]

