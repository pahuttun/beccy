# Instructions how to install Fuse and required tools for Mac

These instructions are ment for people with macOS.

Go with the easy way unless...
- There is not yet a Mac port for latest version of Fuse
- And you really really really need a latest version of Fuse

Instructions have been tested with macOS High Sierra

## The easy way: Mac port

Install the latest version of the Fuse and Fuse utils for macOS
- [Download application](https://sourceforge.net/projects/fuse-for-macosx/)
- Unpack the tar
- Read the README for up-to-date installation instructions

## The hard way: Install from source files

Install the latest version of these 3 programs in this order by downloading and unpacking the tar file:
- [Fuse utilities](https://sourceforge.net/projects/fuse-emulator/files/fuse-utils/)
- [Libspectrum](https://sourceforge.net/projects/fuse-emulator/files/libspectrum/)
- [Fuse](http://fuse-emulator.sourceforge.net/)

For every program, obey the installation instructions. Always check the output after `./configure` as it will tell what requirements you are missing.

## The optional way: Virtual linux

Virtual Linux is good choice if you want to encapsulate everything to virtualized environment and/or want to install Fuse from source.

Follow these two easy steps:
1) [Install virtual Linux](virtual-linux.md)
2) [Follow installation instructions for Linux](installation-linux.md)

## Problems I've encountered

### SOLVED: The hard way - Libspectrum: Glib not found

Problem:
`configure: error: Glib not found`

Solution:
- Run: `./configure --with-fake-glib`

### UNSOLVED: The hard way - Fuse: Installation failed because of missing libraries

The installation of Fuse failed because of missing libraries. Unfortunately, I didn't find solution for these problems and because the Mac port is the latest version and it bundles all utilities, I followed that route.
