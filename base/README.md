# Base Dockerfile

A Dockerfile for the base image. This is image will serve as a starting point for all other images
in this repository.

## Dependencies

[ubuntu]

## Installation

Install [Docker], then

### Install using the Docker Registry

`sudo docker pull pseudomuto/base`

### Clone and Build

```
git clone https://github.com/pseudomuto/dockerfiles.git
rake build[base]
```

[Docker]: https://www.docker.io/
[ubuntu]: https://registry.hub.docker.com/_/ubuntu/
