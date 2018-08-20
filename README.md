# Beccy - The beginners instructions for Spectrum development

When I was a kid I had Spectrum ZX and I was spending all my evenings developing little games and software. Fast forward 30 years. "Hey, I should create a fun little game for Spectrum", I was thinking while pooping. It cannot be so hard!

Well, maybe it wasn't so hard, but I was a bit frustrated to get things started and rolling. What are the prerequisities to get my first Hello World program done? What kind of software I need? How can I write software with my Mac and then run it in Spectrum emulator?

This project will answer these questions.

## Getting Started

I'm a Mac user but decided to use Ubuntu 18.04 LTS for this project. The main reason is that although there are Mac ports of the emulator we will be using, it seems that the latest version is currently Linux only.

Notice: All instructions are written assuming that you have Ubuntu 18.04 LTS. Your mileage might vary with other distros.

### Prerequisites

List of prerequisities:
- Ubuntu 18.04 LTS or similar
- Spectrum emulator
	- Fuse (1.5.6 used)
	- Fuse utils (1.4.3 used)
	- libspectrum (1.4.4 used)

Fear not, you can find the installation instructions below.

#### Optional: Install latest Ubuntu for Mac

Installing virtualized Linux for Mac is quite straightforward and I won't go into the details.

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
6) Power on and good luck! Obey the Linux instructions for installation
	- Notice: These instructions assume that you do the Minimal installation when it asks. If you plan to use this virtual Linux for other user than Spectrum emulator development, do the Normal installation

#### Optional: Prerequirements of Spectrum emulator for fresh Ubuntu installs

If you have just installed the Ubuntu with minimal installation, there are some tasks you need to do before you can install the Spectrum emulator.

List of prerequirements:
- 

#### Install Spectrum emulator Fuse and required 

### Installing

A step by step series of examples that tell you how to get a development env running

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
