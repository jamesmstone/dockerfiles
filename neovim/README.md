# neovim
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/neovim.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/neovim)

A dockerised version of neovim
## Usage
`docker run -it --rm -v "$(pwd)":/wd -w /wd jamesmstone/neovim`

Alternatively, you can add `alias nvim="docker run -it --rm -v "$(pwd)":/wd -w /wd jamesmstone/neovim"` to your .bashrc or similar.

Inspired by work done here: https://hub.docker.com/r/kr1sp1n/alpine-neovim/
