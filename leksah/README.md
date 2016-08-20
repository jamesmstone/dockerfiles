# leksah
 [![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/leksah.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/leksah/)
 
A dockerised version of [Leksah](http://leksah.org/)
## Usage
```
docker run -d --rm \
	-v /etc/localtime:/etc/localtime:ro \
	-v /tmp/.X11-unix:/tmp/.X11-unix \
	-e DISPLAY=unix$DISPLAY \
	-v "$(pwd)":/home/root \
	-e GDK_SCALE \
	-e GDK_DPI_SCALE \
	--name leksah \
	jamesmstone/leksah
```
