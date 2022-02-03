all: build

build:
	ghc --make -fllvm -O2 -XBangPatterns -threaded -rtsopts -fforce-recomp -funbox-strict-fields -XScopedTypeVariables main.hs -o knucleotide
