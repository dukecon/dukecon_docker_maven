FROM maven:3.6.3-adoptopenjdk-14
MAINTAINER Gerd Aschemann <gerd@aschemann.net>

RUN apt-get update && apt-get -qq dist-upgrade
RUN apt-get install -qq -y git
RUN apt-get install -qq -y glib-2.0 libgconf-2-4 chromium-browser bzip2
RUN apt-get install -qq -y iceweasel
RUN apt-get install -qq -y xvfb
RUN apt-get install -qq -y graphviz
RUN apt-get autoremove -qq

COPY settings.xml /usr/share/maven/conf
