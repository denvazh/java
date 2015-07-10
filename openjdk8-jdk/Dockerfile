# Debian 8.1 with OpenJDK Java Runtime Environment 8

FROM debian:8.1

MAINTAINER Denis Vazhenin <denis.vazhenin@me.com>

ENV BACKPORTS "deb http://httpredir.debian.org/debian jessie-backports main contrib non-free"

RUN echo "$BACKPORTS" > /etc/apt/sources.list.d/jessie-backports.list && \
    apt-get update && \
    apt-get -t jessie-backports install openjdk-8-jdk -y

# Expose reference to JAVA_HOME
ENV JAVA_HOME /usr/lib/jvm/java-8-openjdk-amd64
