# MTASC

The SWFRecomp fork of MTASC from SourceForge.

## Building

### Windows

If you are on Windows...please do not try to use native `opam` to build this. 🫠 You will die.

It is advised to use WSL to test contributions, following the steps below.

### Linux (or WSL)

To build this repo, you first need to acquire `opam`, the OCaml package manager.

https://ocaml.org/docs/installing-ocaml

After initializing `opam` with `opam init -y`, simply `cd` to this repo and run:

```
opam update
opam switch create 3.11.2
eval $(opam env --switch=3.11.2)
make
```