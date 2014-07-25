# Redis Slave Dockerfile
#
# https://github.com/pseudomuto/dockerfiles/tree/master/redis_slave
#

FROM pseudomuto/base_redis
MAINTAINER David Muto <david.muto@gmail.com>

# Update to invalidate image cache
ENV PMDF_REFRESHED_AT 20140724003411

ENTRYPOINT ["redis-server", "--slaveof redis_master 6379"]
CMD ["--logfile /var/log/redis/redis-%H.log"]
