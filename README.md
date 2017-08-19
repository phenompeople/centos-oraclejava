[![Build Status](https://travis-ci.org/phenompeople/centos-oraclejava.svg?branch=master)](https://travis-ci.org/phenompeople/centos-oraclejava)
Oracle JDK & JRE
===============

Dockerfiles for building a Java base images.

The images are available directly from [phenompeople organization] (https://hub.docker.com/u/phenompeople/)

**Which Java container do i need?**

**JDK (Java SE Development Kit)** For Java Developers. Includes a complete JRE plus tools for developing, debugging, and monitoring Java applications.
**Server JRE (Server Java Runtime Environment)** For deploying Java applications on servers. Includes tools for JVM monitoring and tools commonly required for server applications, but does not include browser integration (the Java plug-in), auto-update, nor an installer. Covers most end-users needs. Contains everything required to run Java applications on your system.

### Supported tags and respective `Dockerfile` links

#### phenompeople/sunjdk

* **`8u144` ([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-sunjdk/src/master/jdk/8u144/Dockerfile))**
* **`8u131` ([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-sunjdk/src/master/jdk/8u131/Dockerfile))**

#### phenompeople/sunjre

* **`8u144` ([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-sunjdk/src/master/jdk/8u144/Dockerfile))**
* **`8u131` ([jdk/8u131/Dockerfile](https://bitbucket.org/phenompeople/centos-sunjdk/src/master/jdk/8u131/Dockerfile))**

**NOTE:** `centos-sunjdk` and `centos-sunjre` provides only the base images which are build on ONBUILD instructions. The ONBUILD instruction adds to the image a trigger instruction to be executed at a later time, when the image is used as the base for another build.

#### Pre-Requisites

- install docker-engine [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/)

#### Usage of `onbuild` images

These images can be used to bake your dependencies into an image by extending the plain storm images. To do so, create a custom `Dockerfile` like this:
```dockerfile
FROM phenompeople/centos-sunjdk
```
Don't forget to build that `Dockerfile`:
```
docker build --rm=true -t childimage .
```
```
docker run --rm -t childimage
```
## Maintainers

* Rajesh Jonnalagadda (<rajesh.jonnalagadda@phenompeople.com>)

## License and Authors
**License**	::		Apache License
**Author**	::		Phenompeople Pvt Ltd (<admin.squad@phenompeople.com>)