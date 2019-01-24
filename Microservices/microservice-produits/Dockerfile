from ubuntu:latest
RUN \
# Update
apt-get update -y && \
# Install Java
apt-get install openjdk-8-jdk -y
ADD ./target/mproduits-0.0.1-SNAPSHOT.jar produits.jar
EXPOSE 9001
CMD java -jar produits.jar