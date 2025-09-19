FROM openjdk:21

COPY src/main/java/org/OlaUnicamp.java /app/org/OlaUnicamp.java

WORKDIR /app

RUN javac org/OlaUnicamp.java

CMD ["java", "org.OlaUnicamp"]