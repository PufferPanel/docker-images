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

RUN         apt-get update && apt-get install -y lib32gcc1 lib32tinfo5 lib32z1 curl tar lib32stdc++6
RUN         useradd -m -d /home/container container

USER        container
ENV         HOME /home/container

WORKDIR     /home/container

CMD         ["/bin/bash"]
