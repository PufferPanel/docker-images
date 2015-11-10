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

RUN         apt-get update && apt-get install -y perl gcc g++ make automake libtool autoconf m4 gcc-multilib
RUN         useradd -m -d /home/container container

USER        container
ENV         HOME /home/container

WORKDIR     /home/container

CMD         ["/bin/bash"]
