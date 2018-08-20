# Beccy - The beginners instructions for Spectrum development

When I was a kid I had Spectrum ZX and I was spending all my evenings developing little games and software. Fast forward 30 years. "Hey, I should create a fun little game for Spectrum", I was thinking while pooping. It cannot be so hard!

Well, maybe it wasn't so hard, but I was a bit frustrated to get things started and rolling. What are the prerequisities to get my first Hello World program done? What kind of software I need? How do I avoid writing the software with the horrible keyboard layout Spectrum has? How to create and run tape files?

This project will answer these questions.

## Install the required software

The following chapter will walk you through the installation of required software to run your own Spectrum programs.

There are instructions for Linux (Ubuntu 18.04 LTS used) and Mac (High Sierra used).

The rest of the instructions assume that you are using Mac version. Most probably the Linux version is quite similar.

### Install the prerequisites: Linux

List of prerequisities we will be installing next:
- libspectrum (1.4.4 used)
- Fuse (1.5.6 used)
- Fuse utils (1.4.3 used)

If you want to use virtualized linux, [read these instructions](docs/virtual-linux.md)

#### Libspectrum

Install the latest version of the Libspectrum
- [Download latest code](http://fuse-emulator.sourceforge.net/libspectrum.php)
- Unpack the tar
- Read the README for up-to-date installation instructions
- Install
	- `./configure`
	- `make`

**Problems I encountered**

`configure: error: Glib not found`
- Run: `./configure --with-fake-glib`

#### Fuse utils

Install the latest version of the Fuse utils
- [Download latest code](https://sourceforge.net/projects/fuse-emulator/files/fuse-utils/)
- Unpack the tar
- Read the README for up-to-date installation instructions
- Install
	- `./configure`
	- `make`

#### Fuse

Install the latest version of the Fuse
- [Download latest code](https://sourceforge.net/projects/fuse-emulator/files/fuse/)
- Unpack the tar
- Read the README for up-to-date installation instructions
- Install
	- `./configure`
	- `make`
	- `make install`

### Install the prerequisites: Mac (High Sierra)

List of prerequisities we will be installing next:
- Fuse for macOS (1.5.6)

#### Fuse for macOS

Install the latest version of the Fuse for macOS
- [Download application](https://sourceforge.net/projects/fuse-for-macosx/)
- Unpack the tar
- Read the README for up-to-date installation instructions

## Test the Fuse UI and create your first program

To make sure your installation is working, let's test the Fuse out by writing our first program. We will be using the UI to do that for now. Later on I'll explain how to use your favourite text editor and create tape files.

### Create 'Hello World' program

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

Now you can decide what you want to learn next:
- Keyboard layout aka "Help, how do I type?"
- Basics of BASIC aka "Help, how to program?"
- How to code with my favorite editor, create and execute tape files
- Tools to help you generating Spectrum software

## Getting started

### Keyboard layout

http://slady.net/Sinclair-ZX-Spectrum-keyboard/

TODO

### Basics of BASIC

TODO

### How to code with my favorite editor

TODO

### Tools to help you

TODO

## Your first project

TODO

## Software used

* [Fuse](http://fuse-emulator.sourceforge.net/) - The Spectrum emulator used
* [Fuse for macOS](https://sourceforge.net/projects/fuse-for-macosx/) - The Spectrum emulator's Mac version
* [Fuse utilities](https://sourceforge.net/projects/fuse-emulator/files/fuse-utils/) - Helpful utilities for emulator
* [Libspectrum](https://sourceforge.net/projects/fuse-emulator/files/libspectrum/) - Helpful input/output utilities for emulator

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Everyone who has ever owned Spectrum ZX
