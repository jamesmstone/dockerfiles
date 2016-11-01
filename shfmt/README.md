# shfmt
 [![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/shfmt.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/shfmt/)

A dockerised version of [shfmt](https://github.com/mvdan/sht)
## Usage
```
docker run -it --rm \
	-v "$(pwd)":/sh \
	-w /sh \
	jamesmstone/shfmt "$@"
```
### One liner
`docker run -it --rm 	-v "$(pwd)":/sh -w /sh 	jamesmstone/shfmt `

### Example
`docker run -it --rm 	-v "$(pwd)":/sh -w /sh 	jamesmstone/shfmt -l -w script.sh`
