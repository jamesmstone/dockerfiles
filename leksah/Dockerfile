FROM haskell
RUN cabal update && \
cabal install Cabal cabal-install &&\
cabal install alex happy && \
cabal install gtk2hs-buildtools && \
cabal install leksah
ENTRYPOINT ["leksah"]
