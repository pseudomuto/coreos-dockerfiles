#
# Base Dockerfile
#
# https://github.com/pseudomuto/dockerfiles/tree/master/base
#

FROM ubuntu:14.04
MAINTAINER David Muto <david.muto@gmail.com>

# Update to invalidate image cache
ENV PMDF_REFRESHED_AT 20140722232113

RUN \
  apt-get update && apt-get -y upgrade && \
  apt-get install -y build-essential curl wget vim git software-properties-common

ENV HOME /root

WORKDIR /root

CMD ["bash"]
