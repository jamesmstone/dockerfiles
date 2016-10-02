
FROM kalilinux/kali-linux-docker
MAINTAINER	James Stone

RUN	apt-get update && apt-get upgrade -y && apt-get install -y \
	--no-install-recommends \
	urlcrazy \
	&& \
	apt-get autoremove && \
	rm -rf /var/lib/apt/lists/*

ENTRYPOINT	["urlcrazy"]
