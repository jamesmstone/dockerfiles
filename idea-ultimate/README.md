# Docker image for IntelliJ IDEA Ultimate.
[![Build Status](https://travis-ci.org/jamesmstone/dockerfiles.svg?branch=master)](https://travis-ci.org/jamesmstone/dockerfiles) [![Docker Pulls](https://img.shields.io/docker/pulls/jamesmstone/idea-ultimate.svg?maxAge=2592000)](https://hub.docker.com/r/jamesmstone/idea-ultimate/)
> **Note:** This is a fork from the original: [dlsniper](https://github.com/dlsniper/)/[docker-intellij](https://github.com/dlsniper/docker-intellij). I made this fork as I was after a version that used the ultimate edition additionally, as I was after as small and fully customizable container this doesn't come with any pre-installed plugins. However, if you mount the `config` dir you can have plugins you download in one session transfer to the next.

The image contains the following software:

- [IntelliJ IDEA Ultimate 2016.1.4](https://www.jetbrains.com/idea/)


## Running

By running the following command you'll be able to start the container

```bash
docker run --rm -it \
           --net="host" \
           --privileged=true \
           -e DISPLAY=${DISPLAY} \
           -v /tmp/.X11-unix:/tmp/.X11-unix \
           -v ${HOME}/.config/idea:/config \
           -v "$(pwd)":/home/root \
           jamesmstone/idea-ultimate
```

The command will do the following:

- save the IDE preferences into `<your-HOME-dir>/.config/idea`
- loads the current dir into the home directory of the current (root) user in the container.

## Updating the container

To update the container, simply run:

```shell
docker pull jamesmstone/idea-ultimate
```

Each of the plugins can be updated individually at any time, and other plugins
can be installed as well.

However, to update IntelliJ IDEA itself, the docker image will need to be
updated.

## License

The MIT License (MIT)

Copyright (c) 2016 Florin Patan

If you want to read the full license text, please see the [LICENSE](https://github.com/dlsniper/docker-intellij/blob/master/LICENSE) file.
IntelliJ IDEA and all the other plugins are or may be trademarks of their
respective owners / creators. Please read the individual licenses for them.
