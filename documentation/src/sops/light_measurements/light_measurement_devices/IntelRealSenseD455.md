 # Standard Operating Procedure for IntelRealsense D455 depth camera

This SOP provides an overview over project specific measurements with the device Intel RealSense D455 for the project ReWoCap. General handling of the device is decribed in another SOP.

| Device       | Intel, Realsense D455                                             |
|--------------|-----------------------------------------------------------|
| Objective    | Describe the measurement with Depth camera D455                     |
| Owner     | [Niloufar Tabandeh](mailto:niloufar.tabandehsaravi@tuebingen.mpg.de) |
| Contributor     | [[Alexander Hahn](mailto:alexander.hahn@tuebingen.mpg.de) |
| Version      | _1.0.1.                                        |
| Last edit    | 12.06.23 |
| Date         | 20.04.23                                                |

## Start up

Checklist for materials
   1. IntelRealsense D455 depth camera SN: 231122300377
   2. Screw for mounting
   4. Intel Realsense software
   5. USB-hub
   6. USB-cable (part of the larger cable unit)
   7. Hard-drive
    
Start up system
   1. Plug the USB-connector-cable into the laptop
   2. Plug the other end of the USB-connector-cable into the D455 (This activates the device)
    

## Pre-measurement procedure

   1. General: Place the entire measurement setup in the desired position
   2. Take the D455 out of its casing from the portable backpack
   3. Use the little screw to attach the D455 to the mounting in the middle left part of the front of the box

## Measurement procedure

   1. Open the Intel Realsense software. The camera is recognized automatically. 
   2. In the upper left panel, click on the modulators next to RGB-camera and Stereo module in the upper left part of the software window. Framerate and resolution stay at default setting.
   3. Set a timer for 15 seconds (e.g. with your cellphone)
   3. Click record in the upper left part of the software window
   3. Stop the recording after 15 seconds
   3. Close the software and reopen shortly before the next measurement
   

## Data Saving

Export/Access Data
    
   1. Data is saved automatically in "Documents".
   2. Automated saving/renaming
        1. Transfer the files into the designated folder that is used by the Python Code for automated renaming (if you don´t know the name of the folder, you can look it up in the header of the code). 
        2. Follow the instructions in the header of the Python-Code and subsequently run the code.
   3. Manual saving/renaming 
        1. Rename each file to inteld455_year:month:dayTmeasurementtime (e.g. inteld455_20230208T0930.bag)
        2. Transfer the renamed file to Hard-Drive &rarr; rewocap &rarr; data &rarr; raw &rarr; ID (e.g., 1001_20230208)
   
## Shut down
   
