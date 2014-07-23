# Redis Master Dockerfile

This Dockerfile is used to create a master (or single) redis instance.

## Dependencies

[pseudomuto/base_redis]

## Installation

Install [Docker]. Then...

### Install using the Docker Registry

`sudo docker pull pseudomuto/redis_master`

### Clone and Build

```
git clone https://github.com/pseudomuto/dockerfiles.git
rake build[redis_master]
```

## Usage

`sudo docker run -d -h <host_name> --name <container_name> pseudomuto/redis_master`

[Docker]: https://www.docker.io/
[Docker Registry]: https://registry.hub.docker.com/
[pseudomuto/base_redis]: https://github.com/pseudomuto/dockerfiles/tree/master/base_redis
