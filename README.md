# Beccy - The beginners instructions for Spectrum development

The goal of this project is to explain how to develop programs for ZX Spectrum, home computer from 1980's, with modern computers.

All the information can be already found from various forums and sites, but the information is scattered. Also, most of the information concentrates on how to program WITH ZX Spectrum, not how to program TO ZX Spectrum. As the Speccy's keyboard layout and programming editor is notoriously horrible, it helps a lot if you can do the hard work with your own computer using IDEs and tools.

## Contents

Expectation management:

- These instructions will tell you how to develop and run programs for ZX Spectrum, "Speccy", the home computer for 1980's
- You will both learn how to program WITH Speccy and how to program TO Speccy using your own computer.
- You will learn how to install required emulators and tools (Linux, Mac, Windows)

Index:

- **Contents** of these instructions
- **Install** the required software
- **Hello world**, your first ZX Spectrum program
- **Work with tapes**, how to save/load tape files
- **Basics of BASIC**, dive to Spectrum's own programming language
- **Assembler**, this is where the magic happens
- **Programming workflow**, instructions how to code with your own computer instead of Speccy

## Install the required software

Before starting, we need to install required software for ZX Spectrum emulation and programming:
- ZX Spectrum emulator: Fuse will be used
- Required libraries and tools for Fuse
- Additional tools that enables you to program with your own computer

Installation instructions are here:

- [Installation instructions for Linux](docs/installation-linux.md)
- [Installation instructions for Mac](docs/installation-mac.md)
- [Installation instructions for Windows](docs/installation-windows.md)


## Create your first 'Hello World' program

Open the application and you should be greeted with gray box. You are ready to start typing your first program.

Notice, that the keyboard layout is really wonky and you most probably will need help with that.

First, read this: <http://slady.net/Sinclair-ZX-Spectrum-keyboard/>

You get different output from same keys depending on which **keyboard mode** you are. Also, instead of typing the commands, **keywords** are added by just pressing one key.

Confusing? Yes, it is.

Try to write the following code:
```
10 PRINT "HELLO WORLD"
RUN
```

Instructions how to do that:

- Type 10 (we'll discuss line numbers later)
- Press P for PRINT
- Press Alt+P for opening " (notice: check your keyboard layout if ALT doesn't work)
- Type HELLO WORLD
- Press Alt+P for closing "
- Press Enter
- Press R for RUN and Enter to execute your program

You should see `HELLO WORLD` and `0 OK, 10:1`

Congratulations, your first Spectrum program is now ready!


## Storing and restoring data: fun with tapes

Before even touching the subject of "How to code", let's start first understanding how to read and store data using manually operated or fully automated virtual tape files.

If you are interested, please read the [background information of ZX Spectrum storage formats and peculiarities](docs/theory-storage.md).

There are two different methods of using tapes:

- Virtual cassette player emulator
- Tape files

### Let's learn: using virtual cassette player emulator

Fuse is equipped with virtual cassette player emulator. Good news: everything is virtual. Bad news: you still need to operate it manually.

**Tutorial: Saving the program to virtual tape and validating that it loads**

Type in the hello world program if you haven't done so. `RUN` it to test that it works.

Save it with a following command:
`SAVE "hello"` (tip: key S = SAVE, ALT+P = ")

You should see:
`Start tape, then press any key`

Do as commanded:

- Select from Fuse's menu: Media => Tape => Record start
- Press any key
- Watch the beep-bleep color show until you get `0 OK, 0:1`
- Stop the recording: Media => Tape => Record stop

You have just recorded the program to virtual tape. Congratulations!

To test whether you were succesful, do following:

- `NEW` (tip: A = NEW)

    ZX Spectrum should show a black box for a moment, as it restarts itself. Your program should be now gone.

- `RUN`

    You shouldn't see hello world anymore. Your program is actually gone.

- `LOAD "hello"` (tip: J = LOAD)

    You should see `Program: hello`

- `RUN`

    Ta-dah! Your program is here again!

Actually, the exercise above wouldn't have worked with the real cassette player, at least not with every model. The reason for that is that we didn't rewind the tape after saving it.

Fortunately, Fuse's virtual cassette player is so intelligent that it automatically loops the cassette. When the end is reached, it automatically instantly rewinds the cassette and starts from beginning.

**Tutorial: Saving the virtual tape to tape file**

You have stored your program to virtual tape, but that tape is disposable and will be lost when you close emulator.

To actually store the bits, you need to save the virtual tape to tape file.

Do following:

- Media => Tape => Write
- Notice: If you get error `fuse: error: libspectrum: skip_block: skipping RLE Pulse (ID 0x100); conversion almost certainly won't work`, do following:
	- TODO

### Tape files

TODO


## Programming workflow

TBD

## Basics of BASIC

TBD

## Assembler

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
