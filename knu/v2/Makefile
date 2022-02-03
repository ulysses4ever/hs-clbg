all: build run

build:
	ghc -prof -fllvm -O2 -threaded -rtsopts -fforce-recomp -XBangPatterns -XBinaryLiterals -XDerivingStrategies -XGeneralizedNewtypeDeriving -XOverloadedStrings -XScopedTypeVariables -XTypeApplications main.hs -o knu

run:
	./knu +RTS -N4 -K2048M -RTS 0 < ../knu-25000000.txt

deps:
	cabal install -p --lib --package-env=.         \
                        bytestring            \
                        unordered-containers  \
                        parallel-io           \
                        text-builder          \
                        hashable              \
                        vector-algorithms     \
                        vector                \
                        pvar                  \

