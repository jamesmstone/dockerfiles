FROM	golang:alpine
RUN	apk add --no-cache \
	--virtual \
	.build-deps \
	git \
	&& go get -u mvdan.cc/sh/cmd/gosh \
	&& apk del .build-deps git
ENTRYPOINT	["shfmt"]
