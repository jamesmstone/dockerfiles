# xsser
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/xsser.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/xsser)

A dockerised version of [xsser](http://xsser.sourceforge.net/)
## Usage
`docker run --rm -v "$(pwd)":/wd -w /wd jamesmstone/xsser`

Alternatively, you can add `alias xsser="docker run --rm -v "$(pwd)":/wd -w /wd jamesmstone/xsser"` to your .bashrc or similar.
