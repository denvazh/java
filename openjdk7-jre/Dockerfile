# Alpine Linux with OpenJDK Java Runtime Environment 7

FROM gliderlabs/alpine:3.1

MAINTAINER Denis Vazhenin <denis.vazhenin@me.com>

RUN apk-install bash openjdk7-jre-base ca-certificates && \
  find /usr/share/ca-certificates/mozilla/ -name *.crt -exec keytool -import -trustcacerts \
  -keystore /usr/lib/jvm/java-1.7-openjdk/jre/lib/security/cacerts -storepass changeit -noprompt \
  -file {} -alias {} \; 2>&1>/dev/null && \
  keytool -list -keystore /usr/lib/jvm/java-1.7-openjdk/jre/lib/security/cacerts --storepass changeit

# Expose reference to JAVA_HOME
ENV JAVA_HOME /usr/lib/jvm/java-1.7-openjdk