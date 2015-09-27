# ##
# Docker: SRCDS
#
# Builds a docker image for running a steamcmd based server on PufferPanel.
#
# Author: puffrfish
# ##

FROM        ubuntu:14.04

MAINTAINER  puffrfish <puffrfish@puffrfish.com>

ENV         DEBIAN_FRONTEND noninteractive

RUN         apt-get update && apt-get install -y lib32gcc1 lib32tinfo5 curl tar
RUN         mkdir -p /data/steamcmd && cd /data/steamcmd
RUN         curl -O https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz
RUN         tar -xzvf steamcmd_linux.tar.gz && rm -rf steamcmd_linux.tar.gz

EXPOSE      27015

WORKDIR     /data

CMD         ["/bin/bash"]
