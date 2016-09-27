# Weka
 [![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/weka.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/weka/)
 
A dockerised version of [Weka](http://www.cs.waikato.ac.nz/ml/weka/)
## Usage
### GUI
```
docker run --rm \
	-v "$(pwd)" \
	-w "$(pwd)" \
	-e DISPLAY=$DISPLAY \
	-v /tmp/.X11-unix:/tmp/.X11-unix \
	jamesmstone/weka "$@"
```
