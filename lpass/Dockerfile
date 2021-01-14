	
FROM	alpine:latest	AS	builder
RUN	apk add --no-cache \
	--update \
	--upgrade \
	--repository \
	https://dl-cdn.alpinelinux.org/alpine/edge/testing \
	--virtual \
	.build-deps \
	git \
	make \
	cmake \
	gcc \
	build-base \
	pkgconfig \
	libxml2-dev \
	openssl-dev \
	curl-dev \
	openssl \
	libcurl \
	libxml2 \
	pinentry \
	xclip \
	xsel \
	&& git clone --recursive https://github.com/lastpass/lastpass-cli.git /lastpass-cli \
	&& cd  /lastpass-cli \
	&& make install
FROM	alpine:latest
RUN	apk add --no-cache \
	--update \
	--upgrade \
	--repository \
	https://dl-cdn.alpinelinux.org/alpine/edge/testing \
	openssl \
	libcurl \
	libxml2 \
	pinentry \
	xclip \
	xsel
COPY	/lastpass-cli/build/lpass	/usr/local/bin/lpass
ENTRYPOINT	["lpass"]
