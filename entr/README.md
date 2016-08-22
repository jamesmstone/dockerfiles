# entr 
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/entr.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/entr)

A dockerised version of [entr](http://entrproject.org/)
## Usage
`docker run --rm -v "$(pwd)":/wd -w /wd jamesmstone/entr`

Alternatively, you can add `alias entr="docker run --rm -v "$(pwd)":/wd -w /wd jamesmstone/entr"` to your .bashrc or similar.
Examples of using entr can be seen on entr's [website](http://entrproject.org/) 
