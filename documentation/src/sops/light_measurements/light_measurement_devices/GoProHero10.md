# Standard Operating Procedure for GoPro Hero 10

| Device       | GoPro, Hero 10                                            |
|--------------|-----------------------------------------------------------|
| Objective    | High resolution images and videos.                        |
| Owner        | [Niloufar Tabandeh](mailto:niloufar.tabandehsaravi@tuebingen.mpg.de)  |
| Contributor     | [Alexander Hahn](mailto:alexander.hahn@tuebingen.mpg.de) |
| Version      | _Start with 1.0.1_                                        |
| Last edit    | 12.06.23  |
| Date         | 18.04.23                                                |

## Start up

The device can be started by pressing a large buttion on the top of the device. If your cellphone has been previously connected to the GoPro Hero 10 you can also start it via bluetooth using the "Quik" App. 

Checklist for materials
   1. GoPro Hero 10
   1. Battery
   1. microSD card
   1. Charger
   1. Quik App (Downloadable on Android and iOS app stores) 

Start up system (by hand)
   1. Press power button on the left side of the device 

Start up system (remotely)
   1. Start the Quik App on your mobile device (Press "continue as guest" and then the icon "GoPro". If your GoPro has been connected previously, it will find the device and give you the option for connecting)
   


## Preparation

Before working with the GoPro, make sure that the battery is fully charged beforehand, since it depleads very fast while the GoPro is turned on. Also, make sure to have put a microSD with a large storage capacity inside the GoPro Hero 10. This can be done by opening the slider on the side of the device, revealing the battery and the slot for the microSD card. Put the card in with the conducting side facing away from the battery. The card can be retrieved from the slot by slightly pushing it furhter inside the slot.


## Experiment Procedure

In our project, we strive to measure consecutively in intervalls without having to moving the the GoPro Hero 10. The prefered way of operating in this way is remotely via the Quik app. Turing the GoPro off in between measurements is also adviced, since the battery depleads very fast. 

   1. Position the GoPro at the desired location
   1. Adjust the GoPro in its mounting. This done with two hinges at the bottom of the GoPro, which can be extended and be put in the mounting. A screw (M5) is then used to fasten the hinges in the mounting, thus fixating the GoPro.
   1. Turn on the GoPro via the Quik App
   1. At the preferred time, take a GoPro picture and/or a GoPro video via the App
   1. Turn off the GoPro at the preferred time, using the App



## Data Saving


Export/Access Data
   1. Open the slide on the side of the GoPro Hero 10 and take out the microSD card
   1. If your storage device does not have a slot for a microSD card, use a SD-to-microSD-adapter to connect the microSD carf to your device
   1. Export the preferred data. The videos are saved as .mp4-files and photos as .jpg-files. Besides these, .THM-, .GPR- and .LVM-files are also exportable. 
   		1. THM-files are a scaled down image format for thumbnails (160x120 pixels). 
		2. GPR-files are compressed image-files that contain more data, allowing for improved picture quality. 
		3. LRV-file is a low-quality video file, that is used for showing previews on the mobile App "Quik".
   1. Save the mp4.-, the JPG.-, and the GPR-files in the folder, which is used by the Python-Code for automated saving and renaming of the files. If you do not have access to the code or the code does not work, please save data manually according to the following guideline: 
   		1. Save the data in Hard Drive&rarr;rewocap&rarr;data&rarr;raw&rarr;ID-date&rarr;(e.g., 1001_20230208)&rarr;ID-time (e.g., 1001_20230208T0800) with the file names according to the naming instructions below.
   		2. GPR-files are saved as "gopro10photo_year:month:day:T:time.GPR" (e.g. gopro10photo_20230310T0930.GPR)
   		3. JPG-files are saved as "gopro10photo_year:month:day:T:time.JPG" (e.g. gopro10photo_20230310T0930.JPG)
   		4. mp4-files are saved as "gopro10video_year:month:day:T:time.mp4" (e.g. gopro10video_20230310T0930.mp4)
   3. Alternatively: Delete copied data to free up storage on the microSD-card


## Shut down

The GoPro Hero 10 can be turned off via the Quik App (On/Off button) or the physical black button on left side of the device. Upon turning off, the camera will produce five high pitched beeping-noises.
