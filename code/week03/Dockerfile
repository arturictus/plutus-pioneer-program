FROM haskell:8
RUN apt-get update -y && apt-get install -y libsodium-dev pkg-config

COPY . .
RUN ls
WORKDIR code/week03
RUN ls
RUN cabal update && cabal install --lib

CMD ["cabal", "repl"]
