all: build run

build:
	ghc  --make -fllvm -O2 -XBangPatterns -threaded -rtsopts -funfolding-use-threshold=32 -XMagicHash -XUnboxedTuples main.hs -o revcomp

run:
	./revcomp +RTS -N4 -RTS 0 < revcomp-input250000.txt

# end
