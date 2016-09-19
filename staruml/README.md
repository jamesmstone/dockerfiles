# starUML
 [![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/staruml.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/staruml/)

> **Note:** This is a fork from the original: [huggosantos](https://github.com/huggosantos)/[myDockers](https://github.com/huggosantos/myDockers/tree/master/starUML/2.6.0). I made this fork as I was after an update to their version. Unffortunately, the [pull request](https://github.com/huggosantos/myDockers/pull/1) wasn't approved.
 
A dockerised version of [starUML](https://staruml.io)
## Usage
```
docker run -it --rm \
	-v "$(pwd)":/starUML \
	-w /starUML \
	-v /etc/group:/etc/group:ro \
	-v /etc/passwd:/etc/passwd:ro \
	-v /etc/shadow:/etc/shadow:ro \
	-v /etc/sudoers.d:/etc/sudoers.d:ro \
	-v /tmp/.X11-unix:/tmp/.X11-unix:rw \
	--name staruml \
	jamesmstone/staruml "$@"
```
