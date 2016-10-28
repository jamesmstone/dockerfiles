	
	
	
	
FROM	ubuntu:14.04

RUN	apt-get update && apt-get install -y \
	-q \
	axel \
	xorg \
	unzip \
	dpkg \
	libglib2.0-0 \
	libx11-6 \
	libcairo2 \
	libpango-1.0-0 \
	libpangocairo-1.0-0 \
	libgtk2.0-0 \
	xdg-utils \
	wget \
	libasound2 \
	libgconf-2-4 \
	libnspr4 \
	libnss3 \
	libpango1.0-0 \
	libcurl3

RUN	axel http://staruml.io/download/release/v2.7.0/StarUML-v2.7.0-64-bit.deb
RUN	dpkg -i StarUML-v2.7.0-64-bit.deb


CMD	["/opt/staruml/staruml"]
