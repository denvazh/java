# Alpine Linux with OpenJDK Java Runtime and Development Environment 7

FROM gliderlabs/alpine:3.1

MAINTAINER Denis Vazhenin <denis.vazhenin@me.com>

RUN apk-install bash openjdk7

# Expose reference to JAVA_HOME
ENV JAVA_HOME /usr/lib/jvm/java-1.7-openjdk

# Adjust PATH to include all JDK related executables
ENV PATH $JAVA_HOME/bin:$PATH