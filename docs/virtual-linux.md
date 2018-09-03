# Install Ubuntu 18.04 LTS as virtual Linux for Mac or Windows

Installing virtualized Linux for Mac or Windows is quite straightforward and I won't go into the details.

1) Install latest [Virtualbox](https://www.virtualbox.org/)
2) Create virtual machine
	- Name: *Whatever you choose*
	- Type: Linux
	- Version: Ubuntu (64-bit)
	- Memory: more than the default (I use half of my computer's memory)
	- Create a virtual hard disk now
		- VDI
		- Dynamically allocated
		- At least 30 GB
3) Adjust virtual machine settings
	- Go to virtual machine settings
	- General => Advanced
		- Shared Clipboard: Bidirectional
		- Drag'n'Drop: Bidirectional
	- Display
		- Video memory: 128 MB
		- Enable 3D Acceleration
4) Download latest [Ubuntu LTS ISO](https://www.ubuntu.com/download/desktop)
5) Attach the ISO to the virtual machine
	- Go to virtual machine settings
	- Storage
		- Click picture of DVD under the Controller: IDE
		- Click picture of DVD near the Opical Drive text and select the Ubuntu ISO you downloaded
6) Power on and go through the Ubuntu installation
7) Finalize installation
	- Install Guest Additions to enable shared clipboard
		- When your box is running, go to VirtualBox menu and select Devices => Insert Guest Additions CD image...
		- Follow on-screen instructions and reboot when ready

 Now you can jump to [Fuse linux installation instructions](installation-linux.md)