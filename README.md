## Java

This repository contains experimental **Dockerfile** of [Java](https://www.java.com/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/denvazh/java/) based on lightweight [Alpine Linux docker image provided by gliderlabs](https://registry.hub.docker.com/u/gliderlabs/alpine/). This image also includes mozilla trusted ca certificates imported to `cacerts` trusted keystore.

### Base Docker Image

* [gliderlabs/alpine:3.2](https://registry.hub.docker.com/u/gliderlabs/alpine/) for `openjdk7` images
* [gliderlabs/alpine:3.3](https://registry.hub.docker.com/u/gliderlabs/alpine/) for `openjdk8` images

### Tags

* `latest` (default): OpenJDK Java 8 JRE which is an alias to `openjdk-8-jre`
* `openjdk7-jdk`: OpenJDK Java 7 JDK
* `openjdk7-jre`: OpenJDK Java 7 JRE
* `openjdk8-jdk`: OpenJDK Java 8 JDK
* `openjdk8-jre`: OpenJDK Java 8 JRE

### Installation

1. Install [Docker](https://www.docker.com/)

2. Download [automated build](https://hub.docker.com/u/denvazh/java) from public registry: `docker pull denvazh/java`
  
  (alternatively, one can build an image `docker build -t="denvazh/java" github.com/denvazh/java`)
