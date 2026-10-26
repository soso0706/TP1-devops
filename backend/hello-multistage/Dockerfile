# Étape 1 : compilation avec le JDK
FROM eclipse-temurin:21-jdk-alpine
WORKDIR /usr/src
COPY Main.java .
RUN javac Main.java

# Étape 2 : exécution avec la JRE
FROM eclipse-temurin:21-jre-alpine
COPY --from=0 /usr/src/Main.class .
CMD ["java", "Main"]