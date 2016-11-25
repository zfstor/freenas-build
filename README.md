# Building ZFStor

## Requirements

* Your build environment must be  FreeBSD 10.3-RELEASE or later (or FreeBSD 10-STABLE)
(building on FreeBSD 9 or 11 is not supported at this time).

* An amd64 capable processor.  12GB of memory, or an equal/greater amount
  of swap space, is also required.

* An internet connection for downloading source and packages

## Building

Note: All these commands must be run as `root`.

Install the dependencies:

    # make bootstrap-pkgs

Download and assemble the source code:

    # make checkout

Compile the source, then generate the .ISO:

    # make release

Once the build completes successfully, you'll have release bits in the _BE
directory.
