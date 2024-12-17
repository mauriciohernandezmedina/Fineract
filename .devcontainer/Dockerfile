# Contenedor base: Ubuntu 22.04
FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

# Instalar herramientas básicas
RUN apt-get update && apt-get install -y \
    curl wget unzip git nano ca-certificates \
    software-properties-common \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Instalar Java 17
RUN apt-get update && apt-get install -y openjdk-17-jdk && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64

WORKDIR /workspace
