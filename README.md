# ACSAuto

This is an ImageJ macro script to semi-automatically evaluate the anatomical cross-sectional area of ultrasound images. 

We refer to the pre-print publication for detailled information about the processing operations: 


## Installation
in order use the ACSAuto script, it needs to be installed as a plugin in FIJI. If you are not familiar with FIJI and/or need to install it, please take a look at this link: 
https://fiji.sc/ 

There are two ways how to install ACSAuto as a plugin in FIJI: 
1. Clone the git repository: 
```sh
git clone https://github.com/PaulRitsche/ACSAuto
```
Once you have downloaded the ACSAuto .ijm file on your lokal server, you need to open FIJI. Then you need to install the ACSAuto script as a plugin. Choose 'Plugins' -> 'Install' -> select the .ijm file you wish to install (ACSAuto.ijm) -> 'open'. 
Restart FIJI and the ACSAuto plugin will appear at the bootom of the FIJI plugin list and is ready to use.
 
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
The ACSAuto plugin will appear at the bottom of the FIJI plugin list and is ready to use. 

## Usage

In the following, additional information on how to use the ACSAuto script as efficient as possible can be found. The information is structured based on the workflow of the script. For general information on how to use the ACSAuto script please take a look at the supplementary instruction video. 

The evaluation of ultrasound images by ACSAuto script is highly dependent on sufficient contrast between different tissues and homogeneity of grey values. When acquiring ultrasound images, aponeuroses should be clearly distinguishable from muscle tissue, especially at the medial and lateral muscle end.  

Before analyzing ultrasound images, consider adding a Shortcut for the ACSAuto script. Click Plugins in the main menu, choose  ‘Shortcuts’ ->  ‘Add Shortcut’. Now you have to select the ACSAuto plugin and choose a shortcut on the keyboard. This step allows to easily use the ACSAuto plugin via the selected shortcut without choosing it from the plugin pull-down list.

Before you start analyzing your images, test the pre-specified pre-processing parameters. Adapt them to the characteristics of your images. If different, enter them every time you run the script. If batch mode is selected, the pre-processing settings will be applied to all images inside the selected folder. 
Single images can be evaluated by dragging them into the FIJI main menu window and subsequently running the script on the active image. 

Outline-finder starting points using the “Manual” modality should be placed in the middle of the selected outlines as well as near the medial and lateral end (if more than one point must be specified). When analyzing the m. vastus lateralis and the sorting clockwise option is ticked, place the outline-finder starting point in the muscle middle near the superficial aponeurosis. If starting points are placed with too little space between them, suggested outlines might be incorrect and overlap. 

It is possible that, while adjusting the suggested outlines or ROI, the selection vanishes due to a misplaced click. CTRL+SHIFT+E can be used to get the last active selection back on the active image. In case the suggested outlines are inacceptable, a ROI can be manually drawn into the active image. Therefore, the polygon tool must be selected from the FIJI main menu. However, this should be avoided because it would increase the subjective influence of the investigator.

