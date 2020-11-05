# MongoDB-v3-rpi

This repository contains a Dockerfile of [MongoDB](http://www.mongodb.org/) for [Raspberry Pi](https://www.raspberrypi.org/) published to the public [Docker Hub](https://hub.docker.com/repository/docker/treehouses/rpi-mongo).

This Dockerfile is started from [nonoroazoro/rpi-mongo](https://github.com/nonoroazoro/rpi-mongo) but uses
[this MongoDB](https://github.com/ddcc/mongodb/releases). Usually, 32bit machine cannot use MongoDB version3, 
but the container uses the special compiled MongoDB version3 thanks to [Dominic Chen](https://www.dcddcc.com/blog/2018-06-09-building-mongodb-for-32-bit-ARM-on-debian-ubuntu.html).

### Usage
1. Docker CLI

     `docker run -it --init -p 27017:27017 --name mongodb hirotochigi/rpi-mongo:3`
     
[Reference for init flag](https://stackoverflow.com/questions/43122080/how-to-use-init-parameter-in-docker-run)

2. Docker Compose

     `docker-compose up`

### Note

This MongoDB cannot use the default web interface for MongoDB.
 
For more usage details, please refer to [mongo](https://hub.docker.com/_/mongo/).
