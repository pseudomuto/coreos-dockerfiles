# Base Redis Dockerfile

This Dockerfile is used as the base image for redis. It will install a new version of redis from PPA
rather than the old (2.6.x) version shipped with Ubuntu packages.

## Dependencies

[pseudomuto/base]

## Installation

Install [Docker]. Then...

### Install using the Docker Registry

`sudo docker pull pseudomuto/base_redis`

### Clone and Build

```
git clone https://github.com/pseudomuto/dockerfiles.git
rake build[base_redis]
```
## Usage

This image is not intended to be run directly. Check out [pseudomuto/redis_master] for an example.

[Docker]: https://www.docker.io/
[Docker Registry]: https://registry.hub.docker.com/
[pseudomuto/base]: https://github.com/pseudomuto/dockerfiles/tree/master/base
[pseudomuto/redis_master]: https://github.com/pseudomuto/dockerfiles/tree/master/redis_master
