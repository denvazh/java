## Java

This repository contains experimental **Dockerfile** of [Java](https://www.java.com/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/denvazh/java/) based on lightweight [Alpine Linux docker image provided by gliderlabs](https://registry.hub.docker.com/u/gliderlabs/alpine/)

### Base Docker Image

* [gliderlabs/alpine:3.1](https://registry.hub.docker.com/u/gliderlabs/alpine/)

### Tags

* `latest` (default): OpenJDK Java 7 JRE which is an alias to `openjdk-7-jre`
* `openjdk-7-jdk`: OpenJDK Java 7 JDK
* `openjdk-7-jre`: OpenJDK Java 7 JRE

### Installation

1. Install [Docker](https://www.docker.com/)

2. Download [automated build](https://hub.docker.com/u/denvazh/java) from public registry: `docker pull denvazh/java`
  
  (alternatively, one can build an image `docker build -t="denvazh/java" github.com/denvazh/java`)
