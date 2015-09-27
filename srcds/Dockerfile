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

WORKDIR     /data

RUN         apt-get update && apt-get install -y lib32gcc1 lib32tinfo5 curl tar
RUN         mkdir steamcmd

WORKDIR     /data/steamcmd

RUN         curl -O https://steamcdn-a.akamaihd.net/client/installer/steamcmd_linux.tar.gz
RUN         tar -xzvf steamcmd_linux.tar.gz && rm -rf steamcmd_linux.tar.gz

WORKDIR     /data

EXPOSE      27015

CMD         ["/bin/bash"]
