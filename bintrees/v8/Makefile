all: build

build:
	ghc --make -fllvm -O2 -XBangPatterns -threaded -rtsopts -fno-cse -package parallel main.hs -o bintrees
run:
	./bintrees +RTS -N4 -K128M -H -RTS 19 > /dev/null
deps:
	cabal install --package-env . --lib parallel ghc-compact
