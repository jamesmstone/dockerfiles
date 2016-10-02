# sqlmap
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/sqlmap.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/sqlmap)

A dockerised version of [sqlmap](http://sqlmap.org/)
## Usage
`docker run --rm -v "$(pwd)":/wd -w /wd jamesmstone/sqlmap`

Alternatively, you can add `alias sqlmap="docker run --rm -v "$(pwd)":/wd -w /wd jamesmstone/sqlmap"` to your .bashrc or similar.
