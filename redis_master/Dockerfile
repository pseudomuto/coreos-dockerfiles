# Redis Master Dockerfile
#
# https://github.com/pseudomuto/dockerfiles/tree/master/redis_master
#

FROM pseudomuto/base_redis
MAINTAINER David Muto <david.muto@gmail.com>

# Update to invalidate image cache
ENV PMDF_REFRESHED_AT 20140724003411

ENTRYPOINT ["redis-server", "--logfile", "/var/log/redis/redis-master.log"]
