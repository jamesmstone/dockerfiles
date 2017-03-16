# GPS Babel
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/gpsbabel.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/gpsbabel)

A dockerised version of [GPS Babel](https://www.gpsbabel.org)
## Usage
`docker run --rm -it -v "$(pwd)":/wd -w /wd  jamesmstone/gpsbabel`

Alternatively, you can add `alias gpsbabel="docker run --rm -it -v "$(pwd)":/wd -w /wd  jamesmstone/gpsbabel"` to your .bashrc or similar.
