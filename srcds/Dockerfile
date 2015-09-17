# ##
# Docker: SRCDS
#
# Builds a docker image for running a steamcmd based server on PufferPanel.
#
# Author: puffrfish
# ##

FROM        ubuntu:14.04

MAINTAINER  puffrfish <puffrfish@puffrfish.com>

RUN         apt-get update && apt-get install -y lib32gcc1

EXPOSE      27015

WORKDIR     /data

CMD         ["/bin/bash"]
