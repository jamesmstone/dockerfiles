# lpass
[![Build Status](https://travis-ci.org/jamesmstone/dockefiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/lpass.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/lpass/)

A dockerised version of [lpass](https://github.com/lastpass/lastpass-cli), the LastPass CLI
## Usage
`docker run -it -v ${HOME}/.lpass/:/root/.lpass jamesmstone/lpass login`


Alternatively, you can add `alias entr="docker run -it -v ${HOME}/.lpass/:/root/.lpass jamesmstone/lpass"` to your .bashrc or similar.
