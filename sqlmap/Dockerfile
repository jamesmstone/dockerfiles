FROM	kalilinux/kali-linux-docker
MAINTAINER	James Stone

RUN	apt-get update \
	&& apt-get upgrade -y \
	&& apt-get install -y \
	--no-install-recommends \
	sqlmap \
	&& apt-get autoremove -y \
	&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT	["sqlmap"]
