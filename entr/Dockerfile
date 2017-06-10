FROM	debian:latest
MAINTAINER	James Stone

RUN	apt-get update && apt-get install -y \
	--no-install-recommends \
	entr \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT	["entr"]
