# ##
# Docker: Minecraft
#
# Builds a docker image for running a vanilla Minecraft server on PufferPanel.
#
# Author: Dane Everitt
# ##

FROM        buildpack-deps:jessie-scm

MAINTAINER  Dane Everitt <dane@daneeveritt.com>

ENV         DEBIAN_FRONTEND noninteractive
ENV         LANG C.UTF-8

RUN         apt-get -y update
RUN         apt-get -y install default-jre \
                curl \
                openssh-server

EXPOSE      25565

WORKDIR     /data

CMD         ["bash"]
