# Redis Master Dockerfile
#
# https://github.com/pseudomuto/dockerfiles/tree/master/redis_master
#

FROM pseudomuto/base_redis
MAINTAINER David Muto <david.muto@gmail.com>

# Update to invalidate image cache
ENV PMDF_REFRESHED_AT 20140722232113

ENTRYPOINT ["redis-server"]
CMD ["--logfile", "/var/log/redis/redis-master.log"]
