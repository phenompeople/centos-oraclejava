FROM centos:7.3.1611

MAINTAINER Rajesh Jonnalagadda(<admin.squad@phenompeople.com>)
ARG APP_HOME=/opt/deployment
RUN useradd phenom -d ${APP_HOME} -u 1000 && \
    yum install wget -y -q

ARG JAVA_VERSION=8u131
ARG JAVA_DIR=jdk1.8.0_131
ARG JAVA_BUILD=b11

RUN  wget -q -O /tmp/jdk-linux-x64.tar.gz --no-cookies --no-check-certificate --header "Cookie: oraclelicense=accept-securebackup-cookie" \
      "http://download.oracle.com/otn-pub/java/jdk/${JAVA_VERSION}-${JAVA_BUILD}/d54c1d3a095b4ff2b6607d096fa80163/jdk-${JAVA_VERSION}-linux-x64.tar.gz"  && \
     tar -xzf /tmp/jdk-linux-x64.tar.gz -C /usr/local && \
     rm -f /usr/local/${JAVA_DIR}/jdk/{COPYRIGHT LICENSE README THIRDPARTYLICENSEREADME.txt Welcome.html} && \
     ln -s /usr/local/${JAVA_DIR}/bin/java /usr/local/bin && \
     rm -rf /tmp/jdk-linux-x64.tar.gz
ENV JAVA_HOME=/usr/local/${JAVA_DIR}
ENV PATH=$JAVA_HOME/bin:$PATH
