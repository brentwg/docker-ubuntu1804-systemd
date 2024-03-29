# Ubuntu 18.04 LTS - Bionic - Test Image with systemd

[![Build Status](https://travis-ci.org/brentwg/docker-ubuntu1804-systemd.svg?branch=master)](https://travis-ci.org/brentwg/docker-ubuntu1804-systemd) [![Docker Automated build](https://img.shields.io/docker/cloud/automated/brentwg/docker-ubuntu1804-systemd.svg)](https://cloud.docker.com/repository/docker/brentwg/docker-ubuntu1804-systemd) [![Docker Automated build](https://img.shields.io/docker/cloud/build/brentwg/docker-ubuntu1804-systemd.svg)](https://cloud.docker.com/repository/docker/brentwg/docker-ubuntu1804-systemd/builds)

Ubuntu 18.04 LTS (Bionic) Docker container with systemd for testing basic validation of bash automation scripts.

## Prerequisite for Building

Ensure that [Docker](https://docs.docker.com/install/) is installed.

## Quickstart - Building

I use Docker Hub to automatically build a new image whenever the upstream OS container is rebuilt, and any time I push new commits or merge to the 'master' branch. However, to manually build this image, run the following command:

```
docker build -t ubuntu1804-systemd .
```

## Quickstart - Running

To run a container from this image:
```
docker run --detach --privileged --volume=/sys/fs/cgroup:/sys/fs/cgroup:ro brentwg/docker-ubuntu1804-systemd:latest
```

