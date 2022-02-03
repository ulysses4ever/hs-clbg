all: build run

build:
	ghc --make -fllvm -O2 -fforce-recomp -XBangPatterns -threaded -rtsopts -XMagicHash -XUnboxedTuples main.hs -o mandelbrot

run:
	 ./mandelbrot +RTS -s -N4 -RTS 1600 > res
#

# end
