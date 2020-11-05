# Pull base image
FROM balenalib/raspberry-pi:stretch

# Install Java.
RUN apt-get update && apt-get install -y openjdk-8-jdk 

# Define working directory.
WORKDIR /data

# Define default command.
CMD ["bash"]
