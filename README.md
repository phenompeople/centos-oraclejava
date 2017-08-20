[![Build Status](https://travis-ci.org/phenompeople/centos-oraclejava.svg?branch=master)](https://travis-ci.org/phenompeople/centos-oraclejava)
[![Docker Automated build](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://travis-ci.org/phenompeople/centos-oraclejava)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Oracle JDK & JRE

Dockerfiles for building Centos based Oracle Java images.

The images are available directly from [phenompeople organization] (https://hub.docker.com/u/phenompeople/)

**Which Java container do i need?**

**JDK (Java SE Development Kit)** For Java Developers. Includes a complete JRE plus tools for developing, debugging, and monitoring Java applications.
**Server JRE (Server Java Runtime Environment)** For deploying Java applications on servers. Includes tools for JVM monitoring and tools commonly required for server applications, but does not include browser integration (the Java plug-in), auto-update, nor an installer. Covers most end-users needs. Contains everything required to run Java applications on your system.

### Supported tags and respective `Dockerfile` links

#### phenompeople/centos-sunjdk

* **`latest`		([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u144/Dockerfile))**
* **`8u144` 		([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u144/Dockerfile))**
* **`8u131` 		([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u131/Dockerfile))**
* **`services`	([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u131/Dockerfile))**

#### phenompeople/centos-sunjre

* **`latest` 	([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u144/Dockerfile))**
* **`8u144` 		([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u144/Dockerfile))**
* **`8u131` 		([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u131/Dockerfile))**
* **`services` ([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-oraclejava/src/master/jdk/8u131/Dockerfile))**

#### Pre-Requisites

- install docker-engine [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/)

## Maintainers

* Rajesh Jonnalagadda (<rajesh.jonnalagadda@phenompeople.com>)

## License and Authors

**License:**	Apache License

**Author :** Phenompeople Pvt Ltd (<admin.squad@phenompeople.com>)