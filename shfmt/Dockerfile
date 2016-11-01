FROM	golang:alpine
RUN	apk add --no-cache \
	--virtual \
	.build-deps \
	git \
	&& go get -u github.com/mvdan/sh/cmd/shfmt \
	&& apk del .build-deps git
ENTRYPOINT	["shfmt"]
