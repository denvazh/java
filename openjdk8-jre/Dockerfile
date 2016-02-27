# Alpine Linux with OpenJDK Java Runtime Environment 8

FROM gliderlabs/alpine:3.3

MAINTAINER Denis Vazhenin <denis.vazhenin@me.com>

RUN apk-install bash openjdk8-jre-base ca-certificates && \
  find /usr/share/ca-certificates/mozilla/ -name *.crt -exec keytool -import -trustcacerts \
  -keystore /usr/lib/jvm/java-1.8-openjdk/jre/lib/security/cacerts -storepass changeit -noprompt \
  -file {} -alias {} \; && \
  keytool -list -keystore /usr/lib/jvm/java-1.8-openjdk/jre/lib/security/cacerts --storepass changeit

# Expose reference to JAVA_HOME
ENV JAVA_HOME /usr/lib/jvm/java-1.8-openjdk
