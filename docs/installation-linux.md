# Instructions how to install Fuse and required tools for Linux

These instructions are ment for people with Linux and virtual Linux machines.

You can either select the easy way, Flatpak, or the hard way, installing from source.

Why choose hard way?
- At least I personally had lots of problems with Flatpak version and haven't been yet able to solve them. Try the easy way first and if you run into problem, then do the hard way.

## The easy way

### Install the Flatpak, the application installer for Linux

Follow these instructions: https://flatpak.org/setup/
- Select your distro
- Follow at least steps 1, 2 and 4

### Install the Fuse with Flatpak

Install the Fuse with Flatpak:
- [Install and run](https://flathub.org/apps/details/net.sf.fuse_emulator)

## The hard way

### Libspectrum

Install the latest version of the Libspectrum (1.4.4 was used)
- [Download latest code](http://fuse-emulator.sourceforge.net/libspectrum.php)
- Unpack the tar
- Read the README for up-to-date installation instructions
- Install
	- `./configure`
	- `make`
	- `make install` or `sudo make install`
- Make sure to fix encountered problems before moving to next step


### Fuse utils

Install the latest version of the Fuse utils
- [Download latest code](https://sourceforge.net/projects/fuse-emulator/files/fuse-utils/)
- Unpack the tar
- Read the README for up-to-date installation instructions
- Install
	- `./configure`
	- `make`
	- `make install` or `sudo make install`
- Make sure to fix encountered problems before moving to next step


### Fuse

Install the latest version of the Fuse
- [Download latest code](https://sourceforge.net/projects/fuse-emulator/files/fuse/)
- Unpack the tar
- Read the README for up-to-date installation instructions
- Install
	- `./configure`
	- `make`
	- `make install` or `sudo make install`

## Problems I've encountered

### SOLVED: The hard way - Installing libspectrum: no acceptable C compiler

Problem: Running `./configure` gives error `no acceptable C compiler found in $PATH`

Solution: Install build essential package, which includes C compiler

I have minimal installation of Ubuntu 18.04 LTS which is missing some basic tools required for building software. Instead of just installing gcc, it might be wiser to install essential build tools. We will also install pkg-config as it is needed later.

Run: `sudo apt install build-essential`
Run: `sudo apt install pkg-config`


### SOLVED: The hard way - Installing libspectrum: GLib not found

Problem: Running `./configure` gives error `GLib not found`

Solution: Install libgtk-3-dev

Run: `sudo apt install libgtk-3-dev`

### SOLVED: The hard way - Install libspectrum: "bzip2 support: no"

Problem: Running `./configure` shows in summary `bzip2 support: no`

Solution: Install libbz2-dev

Run: `sudo apt install libbz2-dev`

### SOLVED: The hard way - Install libspectrum: "libgcrypt support: no"

Problem: Running `./configure` shows in summary `libgcrypt support: no`

Solution: Install libgcrypt20-dev

Run: `sudo apt install libcrypt20-dev`

### SOLVED: The hard way - Install libspectrum: "libaudiofile support: no"

Problem: Running `./configure` shows in summary `libaudiofile support: no`

Solution: Install libaudiofile-dev

Run: `sudo apt install libaudiofile-dev`

### SOLVED: The hard way - Install Fuse utils: "libjpeg support: no"

Problem: Running `./configure` shows in summary `libjpeg support: no`

Solution: Install libjpeg-dev

Run: `sudo apt install libjpeg-dev`

### UNSOLVED: The easy way - Installing Fuse: failed to load module canberra-gtk-module

Problem: When running the Fuse, you got message: `Gtk-message: Failed to load module "canberra-gtk-module"`

Solution: ???

Already tried:
- (Re)install canberra-gtk-module, didn't work. https://github.com/MajeurAndroid/Adb-Remote-Screen/issues/14
- Install canberra-gtk-module:i386 version, didn't work

### UNSOLVED: The easy way - Keyboard layout: Symbol Shift missing

Problem: You cannot press the "Symbol Shift" button, so some of the commands are not possible to type

Solution: ???

### UNSOLVED: The easy way - Emulator speed suddenly goes to 1000+%

Problem: When switching between Fuse window and other windows, the emulator speed suddenly goes crazy. The % in right corner of the emulator shows numbers over 1000%. Typing is impossible as all key presses are interpreted as 5 or 10 presses

Solution: ???

