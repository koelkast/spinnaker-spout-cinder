# Spinnaker Spout sender in Cinder

Publishes the feed captured with a FLIR (Point Grey) camera via Spout. Tested with the Blackfly S BFLY-PGE-31S4C camera.

Download the binary [here](https://github.com/mediamonks/spinnaker-spout-cinder/releases).

## Running
- Download and install the 64 bit Spinnaker SDK from[ FLIR/Point Grey](https://www.ptgrey.com/support/downloads) (requires creating an account): 
	- Make sure to choose to install the full SDK (don't choose Camera Evaluation)
	- For Visual Studio Version, choose Visual Studio 2015 instead of 2013
- Run the exe

## Developing

### Note about submodules 

When cloning this repository, make sure to recursively check out all submodules. Cinder is included as a submodule and itself contains submodules. 

You can use `git clone --recurse-submodules` on the command line or the submodule options of your GUI git client.

### Note when working with a Visual Studio version higher than 2015
You will need to have the VC++ v140 toolset installed. This can be done for instance with the Visual Studio installer (for instance by going to Programs and Features in the Control Panel, selecting Visual Studio and clicking Change), where you can choose to Modify the installation and check the VC++ v140 toolset checkbox.

### Compiling the binary
Download and install Spout from: http://spout.zeal.co/download-spout/ 

When compiling the binary, make sure that this repository's bin64 folder is in your PATH environment variable.

### Distributing the binary
When distributing the exe, make sure the dlls in the bin64 folder are next to your exe, and there is an `assets` folder containing a `settings.xml` next to the exe.

### Misc
Consider donating to Spout: http://spout.zeal.co/download-spout/



