# Jenkins Docker Slave [Node.js]

[![Travis](https://img.shields.io/travis/jaydp17/jenkins-docker-slave-nodejs.svg)](https://travis-ci.org/jaydp17/jenkins-docker-slave-nodejs)
[![Docker Build Statu](https://img.shields.io/docker/build/jaydp17/jenkins-slave-nodejs.svg)](https://hub.docker.com/r/jaydp17/jenkins-slave-nodejs/)
[![Image Stats](https://images.microbadger.com/badges/image/jaydp17/jenkins-slave.svg)](https://hub.docker.com/r/jaydp17/jenkins-slave-nodejs)
![Contains NPM](https://img.shields.io/badge/contains-npm%40latest-red.svg)
![Contains Yarn](https://img.shields.io/badge/contains-yarn%40latest-blue.svg)

This image takes [jaydp17/jenkins-slave](https://hub.docker.com/r/jaydp17/jenkins-slave/) as base and adds node.js (v6.6 & v7.10) to the image.

Thus it can be used to build node.js projects. It also provides a conenient way to install global packages and use it in your build.

## Usage
### Direct way
Go to `https://<your-jenkins>.com/configure` and directly give `jaydp17/jenkins-slave-nodejs:7.10` as the image in `Docker Image Name`

![Screenshot](screenshot.png)

### Modify the image
If you want to add/ install any more dependencies, you can use this image as base.
```Dockerfile
# Dockerfile
FROM jaydp17/jenkins-slave-nodejs:7.10

# your dependencies/configs go here

```
