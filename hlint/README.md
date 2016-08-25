# HLint
 [![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/hlint.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/hlint/)
 
A dockerised version of [HLint](https://github.com/ndmitchell/hlint)
## Usage
```
docker run -it --rm \
	-v "$(pwd)":/hlint \
	-w /hlint \
	jamesmstone/hlint "$@"
```
