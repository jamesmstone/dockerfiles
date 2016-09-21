	
FROM	haskell
RUN	cabal update \
	&& cabal install hlint \
	&& stack --resolver=nightly install apply-refact
ENTRYPOINT	["hlint"]
