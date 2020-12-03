# ACSAuto

This is an ImageJ macro script to semi-automatically evaluate the anatomical cross-sectional area of ultrasound images. 

We refer to the pre-print publication for detailled information about the processing operations: 


## Installation
To use the ACSAuto script, it needs to be installed as a plugin in FIJI. If you are not familiar with FIJI and/or need to install it, please take a look at this link: 
https://fiji.sc/ 

There are two ways how to install ACSAuto as a plugin in FIJI: 
1. Clone the git repository: 
```sh
git clone https://github.com/PaulRitsche/ACSAuto
```
Once you have downloaded the ACSAuto .ijm file on your lokal server, you need to open FIJI. Then you need to install the ACSAuto script as a plugin. Choose 'Plugins' -> 'Install' -> select the .ijm file you wish to install (ACSAuto.ijm) -> 'open'. 
Restart FIJI and the ACSAuto file will appear at the bootom of the FIJI plugin list and is ready to use.
 
2. Use ImageJ update sites (updates will be automatically installed):

Subsequently to downloading FIJI, you need to add the update site of the ACSAuto script as well as the sites of the depencies. 
Open FIJI and choose 'Help' -> 'Update' -> 'Manage update sites'. Now tick the boxes of the 'BIG-EPFL', 'Biomedgroup', 'ResultsToExcel' and 'UCB Vision Sciences' update sites. 
In doing so, dependencies and update releases will be automatically installed. Scroll to the bottom of the list and click 'Add update site'. A new update site should have been added. 
Modify the details of the new sites with double click: 
```sh
Name: ACSAuto
URL: http://sites.imagej.net/ACSAuto/
Host: webdav:PRitsche
```
After entering the details, ensure ticking the box left of ACSAuto. Choose 'Close' -> 'Apply changes'. Now you have to close and re-open FIJI in order for the newly added plugins to be installed. 
The ACSAuto file will appear at the bottom of the FIJI plugin list and is ready to use. 

## Usage

