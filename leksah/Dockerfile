FROM haskell
RUN	apt-get update && apt-get install -y \
	 libgtksourceview-3.0-dev \
	 libwebkitgtk-3.0-dev \
	--no-install-recommends \
	&& rm -rf /var/lib/apt/lists/* && \

	cabal update && \
	cabal install Cabal cabal-install && \
	cabal update && \
	cabal install alex happy gtk2hs-buildtools && \
	cabal install leksah --allow-newer
ENTRYPOINT ["leksah"]
