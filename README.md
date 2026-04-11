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

### Windows (Cygwin)

...this is not for the faint of heart. If you are contributing, do not waste your time with this.

**Just use WSL.**

But, if you're crazy enough to want to build MTASC as an exe for whatever reason (or you're me from the future when I lose my entire hard-drive LMFAO L DUMBASS) then be my guest, fellow masochist.

Install Cygwin: https://cygwin.com/install.html

From the Cygwin installer (I recommend using the `https://mirror.clarkson.edu` link) install the following packages:

```
rsync
patch
diffutils
curl
make
unzip
git
m4
perl
mingw64-x86_64-gcc-core
mingw64-i686-gcc-core
binutils
mingw64-i686-binutils
```

You may also need any others that OCaml yells at you about while building.

Go to https://fdopen.github.io/opam-repository-mingw/installation/. Download the 64-bit link under Manual Installation.

Run the provided `install.sh` script, and the second provided `opam init` command.

Run the above `opam` commands within the block.

Cross your damn fingers.