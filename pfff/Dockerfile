FROM	ocaml/ocaml:debian

RUN	git clone https://github.com/facebook/pfff.git
RUN	apt-get update && apt-get install -y \
	libgtk2.0-dev \
	libcairo2-dev \
	libpango1.0-dev
RUN	cd /pfff \
	&& ./configure \
	&& make depend \
	&& make \
	&& make opt
ENTRYPOINT	["/pfff/pfff"]
