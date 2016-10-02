# URLCrazy
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/urlcrazy.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/urlcrazy)

A dockerised version of [URLCrazy](http://www.morningstarsecurity.com/research/urlcrazy)
## Usage
`docker run --rm -it -v "$(pwd)":/wd -w /wd  jamesmstone/urlcrazy`

Alternatively, you can add `alias urlcrazy="docker run --rm -it -v "$(pwd)":/wd -w /wd  jamesmstone/urlcrazy"` to your .bashrc or similar.
