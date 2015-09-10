# ##
# Docker: Minecraft
#
# Builds a docker image for running a vanilla Minecraft server on PufferPanel.
#
# Author: Dane Everitt
# ##

FROM        java:openjdk-8

MAINTAINER  Dane Everitt <dane@daneeveritt.com>

RUN         groupadd -r scales && useradd -r -g scales scales

EXPOSE      25565

USER        scales

WORKDIR     /data

CMD         ["bash"]
