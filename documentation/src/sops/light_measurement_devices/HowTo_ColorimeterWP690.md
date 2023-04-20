# Standard Operating Procedure for Westboro Photonics imaging colorimeter WP690

This SOP provides an overview over project specific measurements with the device Jeti Spectoradiometer 1511 for the project ReWoCap. General handling of the device is decribed in another SOP.

| Device       | Westboro Photonics, WP690                                              |
|--------------|-----------------------------------------------------------|
| Objective    | Describe the measurements with WP690             |
| Owner        | [Alexander Hahn](mailto:alexander.hahn@tuebingen.mpg.de)  |
| Reviewer     | [Niloufar Tabandeh](mailto:niloufar.tabandehsaravi@tuebingen.mpg.de) |
| Approver     | [Hannah Heinrichs](mailto:hannah.heinrichs@tuebingen.mpg.de) |
| Version      | _Start with 1.0.0_                                        |
| Last edit    |  |
| Date         | 20.04.23                                                |

## Start up


Checklist for materials
   1. Westboro Photonics Imaging Colorimeter WP690 SN: U006957
   2. Power cabel for power socket (if a power socket is available at the measurement scene)
   3. Power cabel for battery pack outlet (if no power socket is available at the measurement scene)
   4. Westboro Photonics Software on the Laptop
   5. Lense cover
   6. USB-connector (WP690 to Laptop)
   7. Hard-drive
    
    
Start up system
   1. Plugging in the power cable in the thread-outlet on the backside of the device, will automatically start the device. The power cabel for the power socket requires the thread to be thightend. To do this, push the cabel carfully in the socket and tighten the thread for one rotation. Make sure that you hear three beeps from the device and that the diode on the back of the device is green (and not blinking)
   2. Connect the grey USB-cable directly to the PC and not the USB-hub-device
   3. Open the Photometrica software on the Laptop and check whether the device is properly connected via the preview button. The preview button is the green play button in the lower left panel of the workspace. You can test this out with any of the five measurement options (i.e., S-, M-, and L-cone, rhodopsin, and ipRGC)
   4. The first preview often results in an error. Should you get errors in the following previews, the device is not properly connected to the computer or the focal distance is not specified appropriately (the software will complain about something with the mirrors). In case the device is not properly connected, close the Photometrica software and disconnect the WP from the computer. Connect the USB-cable directly to the computer and try opening the software again. Sometimes it can be useful to reconnect the device from the power plug. If you do so, make sure that the Photometrica software is closed beforehand.


## Pre-measurement procedure

   1. General: Place the entire measurement setup in the desired position
   2. Take off the lense cover by pushing the two opposite facing buttons on the side of the lense cover and subsequently pulling it away
   3. Pull up the aluminium handle on the bottom left side (facing the box from the rear) of the black box and extract the light measurement devices to their measurement position (marked by the arrow next to the aluminium handle)
   4. Make sure that the lense is clean. IMPORTANT: Only clean the lense with a specific cloth designed specifically for this porpose. Otherwise the coating of the lense could by damaged.


## Measurement procedure

   1. After you made sure that the device and software are working properly (three beeps + continous green light + Preview did not result in an error) you are ready to start a measurement. 
   2. Import the Outdoor-measurement template. On the bottom right panel is one icon that looks like a folder with a blue arrow pointing upwards (Import)  
   3. --> Desktop/Measurements/Photometrica Templates/Outdoor.PCS . The Outdoor-Template should now by displayed underneath the Circadian-Template.
   4. Start the measurement once the GoPro-Video has started. To do that, hover with the courser over the outdoor-template-panel. A button appears on the outdoor-template-panel, which you can press to start a measurement. Depending on the illuminance of the scene, a measurement typically takes 30-60 seconds.
  


## Data Saving

Export Data
_Two types of data need to be extracted. First, the csv-file. Second, the pmm-file._ 

   1. Make sure that the hard-drive is connected to the laptop via USB.
   1. CSV: Click on the ‘Export data’ tab in the Measurements section (second last icon to the left). A window opens, where you need to select the option csv-file and afterwards the location of storage. 
       Save the data under Hard-Drive&rarr;rewocap&rarr;data&rarr;raw&rarr;ID-date&rarr;(e.g., 1001_20230208)&rarr;ID-time (e.g., 1001_20230208T0800) with the name wp690_year:month:dayTmeasurementtime (e.g. wp690_20230208T0930)
   2. PMM: Click on the ‘Export PMM’ tab in the Measurements section (third last icon to the left). Save the data under Hard-Drive&rarr;rewocap&rarr;data&rarr;raw&rarr;ID (e.g., 1001_20230208) with the name wp690_year:month:dayTmeasurementtime.pmm (e.g. wp690_20230208T0930.pmm)
   3. AFTER THE MEASUREMENT SESSION HAS ENDED, copy the folder ID-date (e.g., 1001_20230208) of the according date to the laptop storage: Desktop &arr; rewocap&rarr;data&rarr;raw
   4. To save storage on the laptop, delete the earliest measurement (according to the ID-date) on the laptop, but only if you have made sure, that this folder is present on the hard-drive.
   5. After you made sure the data is saved, erase the dataset in the software by left-clicking on the orange panel "Outdoor" and right-clicking "Delete". You are then asked if you are sure if you want to delete (click "OK") and afterwards if you want to save a restoring point (click "NO").




## Shut down

   1. Shut down the Photometrica software after making sure no measurement is currently running
   2. Disconnect the WP690 USB-cable from the PC
   3. Disconnect the power cable from the backside of the WP690. If you used battery power, you have to loosen the thread before the cabel can be taken off.
