# Graphics Eclipse
 [![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/graphics-eclipse.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/graphics-eclipse/)

A dockerised version of [Eclipse](https://eclipse.org). I made this version as I needed an image that came with better support for graphics.
## Usage
```
docker run -ti --rm -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix -v "$(pwd)/.eclipse":/home/developer -v "$(pwd)":/workspace --name eclipse jamesmstone/graphics-eclipse
```
