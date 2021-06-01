FROM haskell:8

RUN apt-get update -y && apt-get install -y libsodium-dev pkg-config

COPY . /plutus-pioneer-program
WORKDIR /plutus-pioneer-program/code/week07
RUN cabal update && cabal install --lib

CMD ["cabal", "repl"]
