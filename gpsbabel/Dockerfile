	
	
FROM	alpine:latest

RUN	apk add --no-cache \
	--update \
	alpine-sdk \
	libusb-dev \
	sed \
	qt5-qtbase \
	qt5-qtmultimedia-dev \
	qt5-qttools-dev \
	qt5-qtbase-x11 \
	git \
	&& git clone https://github.com/gpsbabel/gpsbabel.git gpsbabel \
	&& cd gpsbabel \
	&& ./configure \
	&& make \
	&& apk del git make alpine-sdk sed
ENTRYPOINT	["/gpsbabel/gpsbabel"]
