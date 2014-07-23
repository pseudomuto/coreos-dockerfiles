# Base Redis Dockerfile

This Dockerfile is used as the base image for redis. It will install a new version of redis from PPA
rather than the old (2.6.x) version shipped with Ubuntu packages.

## Installation

1. Install [Docker]
2. Download from the [Docker Registry]: `sudo docker pull pseudomuto/base_redis`

## Usage

This image is not intended to be run directly.

[Docker]: https://www.docker.io/
[Docker Registry]: https://registry.hub.docker.com/
