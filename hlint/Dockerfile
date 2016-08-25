FROM haskell
RUN	cabal update && \
	cabal install HLint
ENTRYPOINT ["hlint"]
