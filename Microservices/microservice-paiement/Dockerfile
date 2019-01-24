from ubuntu:latest
RUN \
# Update
apt-get update -y && \
# Install Java
apt-get install openjdk-8-jdk -y
ADD ./target/mpaiement-0.0.1-SNAPSHOT.jar paiments.jar
EXPOSE 9003
CMD java -jar paiments.jar