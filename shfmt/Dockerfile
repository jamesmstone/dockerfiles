FROM	golang:alpine as builder
RUN	apk add --no-cache \
	--virtual \
	.build-deps \
	git \
	&& CGO_ENABLED=0 GOOS=linux go get -u  -a -ldflags '-extldflags "-static"' mvdan.cc/sh/cmd/shfmt \
	&& apk del .build-deps git
ENTRYPOINT	["shfmt"]
FROM scratch
COPY --from=builder /go/bin/shfmt /shfmt
ENTRYPOINT	["/shfmt"]

