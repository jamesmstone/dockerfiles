# SET
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/set.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/set)

A dockerised version of [SET](https://github.com/trustedsec/social-engineer-toolkit/)
## Usage
`docker run --rm -it -v "$(pwd)":/wd -w /wd  jamesmstone/set`

Alternatively, you can add `alias set="docker run --rm -it -v "$(pwd)":/wd -w /wd  jamesmstone/set"` to your .bashrc or similar.
