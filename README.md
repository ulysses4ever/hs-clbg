# Computer Language Benchmarks Game: Haskell

## What

This repo holds (hopefully, up to date) implementations of [the famous CLBG benchmarks
suite][wiki]. Measurements can be seen [on the official site][measures].

[wiki]: https://en.wikipedia.org/wiki/The_Computer_Language_Benchmarks_Game
[measures]: https://benchmarksgame-team.pages.debian.net/benchmarksgame/measurements/ghc.html

Haskell implementations of CLBG has vast prior art, much of which is [reflected on the
Haskell wiki][hwiki]. It is a highly recommended reading if you are interested in diving
into it.

[hwiki]: https://wiki.haskell.org/Benchmarks_Game

## Why

The reason for this repo to exist is that I care about Haskell and various aspects of it.
Due to this, I have been helping in maintaining Haskell implementations of CLBG, including
fixing minor breakages due to GHC updates. I also tried to improve some of them (you can
`grep` through the repo and notice mentions of both kind of contributions).

## How to Contribute

Fixes and improvements to the implementations should be submitted directly upstream, as
issues [against their repo][upstream]. If it's accepted, I'll notice and add it to this
repo. Again, this repo is absolutely secondary to the main repo (referenced above). It's a
convenience for a casual haskeller (me, at least).

[upstream]: https://salsa.debian.org/benchmarksgame-team/benchmarksgame

This repo could use some love in terms of a centralized build system (currently it's just
random Makefiles — mostly because upstream also doesn't accept Cabal or anything like
that). Setting up a CI would be great too.

Some programs are currently missing. Feel free to submit the existing CLBG Haskell 
implementations to this repo.

