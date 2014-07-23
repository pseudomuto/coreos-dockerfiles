# Base Redis Dockerfile
#
# https://github.com/pseudomuto/docker-base
#

FROM pseudomuto/base
MAINTAINER David Muto <david.muto@gmail.com>

# Update to invalidate image cache
ENV PMDF_REFRESHED_AT 20140722232113

RUN \
  apt-get update && apt-get install -y python-software-properties && \
  apt-add-repository ppa:chris-lea/redis-server && \
  apt-get update && apt-get -y install redis-server redis-tools

VOLUME ["/var/lib/redis", "/var/log/redis"]

EXPOSE 6379
