# GNU Radio
 [![Build Status](https://travis-ci.org/jamesmstone/gnuradio.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/gnuradio.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/gnuradio/)

A dockerised version of [GNU Radio](http://gnuradio.org/)
## Tags
This comes in two flavours, `ubuntu` and `alpine` (*Not Working ATM*) 
## Usage
```
docker run --rm -it
  --net="host" \
  -e DISPLAY=${DISPLAY} ] \
  -v /tmp/.X11-unix:/tmp/.X11-unix \
  jamesmstone/gnuradio
```
