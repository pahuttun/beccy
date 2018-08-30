# Beccy - The beginners instructions for Spectrum development

The goal of this project is to explain how to develop programs for Spectrum ZX, home computer from 1980's, with modern computers.

All the information can be already found from various forums and sites, but the information is scattered. Also, most of the information concentrates on how to program WITH Spectrum ZX, not how to program TO Spectrum ZX. As the Speccy's keyboard layout and programming editor is notoriously horrible, it helps a lot if you can do the hard work with your own computer using IDEs and tools.

## Contents

Expectation management:
- These instructions will tell you how to develop and run programs for Spectrum ZX, "Speccy", the home computer for 1980's
- You will both learn how to program WITH Speccy and how to program TO Speccy using your own computer.
- You will learn how to install required emulators and tools (Linux, Mac, Windows)

Index:
- **Contents** of these instructions
- **Install** the required software
- **Hello world**, your first Spectrum ZX program
- **Work with tapes**, how to save/load tape files
- **Basics of BASIC**, dive to Spectrum's own programming language
- **Assembler**, this is where the magic happens
- **Programming workflow**, instructions how to code with your own computer instead of Speccy

## Install the required software

Before starting, we need to install required software for Spectrum ZX emulation and programming:
- Spectrum ZX emulator: Fuse will be used
- Required libraries and tools for Fuse
- Additional tools that enables you to program with your own computer

Installation instructions are here:
- [Installation instructions for Linux](docs/installation-linux.md)
- [Installation instructions for Mac](docs/installation-mac.md)
- [Installation instructions for Windows](docs/installation-windows.md)


## Create your first 'Hello World' program

Open the application and you should be greeted with gray box. You are ready to start typing your first program.

Notice, that the keyboard layout is really wonky and you most probably will need help with that.

First, read this: http://slady.net/Sinclair-ZX-Spectrum-keyboard/

Basically, Spectrum keyboard layout works with "modes". You will get different output from same keys depending on which mode you currently are.

Try to write the following code:
```
10 PRINT "HELLO WORLD"
RUN
```

Instructions how to do that:
- Type 10 (we'll discuss line numbers later)
- Press P for PRINT
- Press Alt+P for "
- Type HELLO WORLD
- Press Alt+P for "
- Type RUN to execute your program

You should see `HELLO WORLD` and `0 OK, 10:1`

Congratulations, your first Spectrum program is now ready!


## Work with tapes

TBD

## Basics of BASIC

TBD

## Assembler

TBD

## Programming workflow

TBD


## Links

### Software used

* [Fuse](http://fuse-emulator.sourceforge.net/) - The Spectrum emulator used
* [Fuse for macOS](https://sourceforge.net/projects/fuse-for-macosx/) - The Spectrum emulator's Mac version
* [Fuse utilities](https://sourceforge.net/projects/fuse-emulator/files/fuse-utils/) - Helpful utilities for emulator
* [Libspectrum](https://sourceforge.net/projects/fuse-emulator/files/libspectrum/) - Helpful input/output utilities for emulator

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Everyone who has ever owned Spectrum ZX
