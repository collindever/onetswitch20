### onetswitch20
This repo stores all Getting-Started projects and reference designs for ONetSwitch20.  

All the documents are provided in MeshSr Wiki.  
Please visit our wiki pages for more information.  
* [ONetSwitch Wiki Home](https://github.com/meshsr/wiki/wiki)  
* [ONetSwitch20](https://github.com/MeshSr/wiki/wiki/ONetSwitch20)
* [Guide for Getting-Started](https://github.com/MeshSr/wiki/wiki/Guide-Getting-Started)  
* [Guide for Reference Design](https://github.com/MeshSr/wiki/wiki/Guide-Reference-Design)  
* [Guide for common Workflow](https://github.com/MeshSr/wiki/wiki/Guide-Workflow)  
* [Hardware Guide ONetSwitch20](https://github.com/MeshSr/ONetSwitch/blob/master/doc/msr-ons20-hwug.pdf)

### Using the Pre-Built Files

These files were run on a ZEDboard using Vitis 2019.2 on an Ubuntu 2019.10 build.

#### Add Boot to SD Card

[Follow this Guide](https://xilinx-wiki.atlassian.net/wiki/spaces/A/pages/18841655/Prepare+Boot+Medium) to copy the `BOOT.BIN` file over to the SD Card. Set the jumper Pins to the follow configuration to boot from the SD Card.

```
MIO 6: set to GND
MIO 5: set to 3V3
MIO 4: set to 3V3
MIO 3: set to GND
MIO 2: set to GND

VADJ Select: Set to 2V5

JP6: shorted
JP2: shorted

All other jumpers should be left unshorted.
```
#### Program Bitstream With Vitis




### Building And Running the Examples

These files were run with Vivado 2019.2 on an Ubuntu 2019.10 build. Block diagram files have been updated to be compatible with Vivado 2019.2 Start by cloning this repo to your local computer.

#### Open Vivado

In the top menu select `Tools>Run Tcl Script` and navigate to one of the subfolders of this repository. From the example subfolder select `/vivado/{example name}.tcl`.  This will create a new Hardware Desgin project for the example.


