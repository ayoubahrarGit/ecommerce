from ubuntu:latest
RUN \
# Update
apt-get update -y && \
# Install Java
apt-get install openjdk-8-jdk -y
ADD ./target/mcommandes-0.0.1-SNAPSHOT.jar commandes.jar
EXPOSE 9002
CMD java -jar commandes.jar