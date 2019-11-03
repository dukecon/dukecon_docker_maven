FROM node:8-slim
MAINTAINER Gerd Aschemann <gerd@aschemann.net>

RUN apt-get update && apt-get -qq dist-upgrade
RUN apt-get install -qq -y git
RUN apt-get install -qq -y glib-2.0 libgconf-2-4 chromium
RUN apt-get install -qq -y iceweasel
RUN apt-get install -qq -y xvfb
RUN apt-get install -qq -y bzip2
# Workaround for JRE installer problem, cf. https://github.com/balena-io-library/base-images/issues/273: Just create dir
RUN mkdir -p /usr/share/man/man1 && apt-get install -qq -y openjdk-8-jre-headless ca-certificates-java
RUN apt-get autoremove
