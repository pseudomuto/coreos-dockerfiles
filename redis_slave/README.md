# redis_slave Dockerfile

This Dockerfile is used to create a redis slave node for a master node. See the [cluster tutorial]
on <http://redis.io/> for more details.

## Dependencies

[pseudomuto/base_redis]

## Installation

Install [Docker]. Then...

### Install using the Docker Registry

`sudo docker pull pseudomuto/redis_slave`

### Clone and Build

```
git clone https://github.com/pseudomuto/dockerfiles.git
rake build[redis_slave]
```

## Usage

```
sudo docker run -d -h <host_name> \
  --name <container_name> \
  --link <master_container_name>:redis_master \
  pseudomuto/redis_slave
```

`<master_container_name>` should be the name of the container running the [redis_master] image.

[Docker]: https://www.docker.io/
[pseudomuto/base_redis]: https://github.com/pseudomuto/dockerfiles/tree/master/base_redis
[redis_master]: https://github.com/pseudomuto/dockerfiles/tree/master/redis_master
[cluster tutorial]: http://redis.io/topics/cluster-tutorial
