# Standard Operating Procedure for the SCENES project measurement with the Compact setup and handling of equipment which is not recorded in another specific device-SOP

This SOP provides an overview of project-specific SCENES measurements with the compact setup.
| Project |SCENES |
|--------------|-----------------------------------------------------------|
| Objective | Describe the measurement procedure of the SCENES project with the compact setup |
| Owner | [Niloufar Tabandeh](mailto:niloufar.tabandehsaravi@tuebingen.mpg.de) |
| Version | _Start with 1.0.1_ |
| Last edit | 19.12.23 |
| Date | 19.12.23 |

## Day before measurement

#### Checklist: Make sure the following devices are fully charged.

1.  Microsoft tablet
2.  2 GoPro Hero 10 batteries (black and white batteries)
3.  Your cellphone

#### Checklist: Make sure the following devices, cables and materials are available

1.  Intel RealSenseD455 depth camera + two screw + cable
2.  GoPro Hero 10 + battery + microSD card + long black screw
3.  Gigahertz Spectroradiometer + cable
4.  Hard drive + USB 3.0 cable
5.  Microsoft tablet + tablet charger
6.  Testo temperature/humidity logger
7.  Memory card reader + USB hub + USB-A to USB-C cable
8.  Tripod + device holder

#### Checklist: Make sure the following procedures are completed

1.  Connect the Microsoft tablet to the internet or manually change to the correct time zone in the tablet's settings.
2.  Check if the Microsoft tablet is fully charged and has sufficient storage capacity.
3.  Put the battery and microSD card inside the GoPro camera. Check that the battery and microSD capacity are sufficient.
4.  Slide down on the GoPro's back screen. Time and date are shown. Then, slide left. In `preferences` section, open the general tab and scroll down to see the `Date` and `Time` tabs. Change them according to the current time zone.
5.  Check that the Testo display shows "REC" for recording

## Day of measurement

_Start half an hour before the first scheduled measurement to creat folders based on convention, check devices and connection and prepare the metadata file_

### Pre-measurement procedure

#### Set up transportation to the location of measurement

1.  Timelapse: Set the tripod and fix it at the desired position.
2.  Trajectory: The devices must be dismounted after each measurement block and carried to different locations.

#### Setting up the equipment

1.  Position the tripod securely at the desired position. Attach devices to the holder.
2.  Attach the GoPro camera, Gigahertz spectroradiometer and Intel depth camera to their holders. Connect the Gigahertz spectroradiometer and Intel depth camera to the Microsoft tablet via cables and USB hub.
3.  Turn on the Microsoft tablet and attach the USB hub.
4.  Turn on the GoPro camera and open the `Quik app` on your cellphone to check their Bluetooth connection.

### Measurement procedures

1.  Follow the device-specific SOPs to perform the measurements (LabHandbook/documentation/src/sops/light-measurement-devices/).
    _All measurements from three devices automatically have been saved on the microSD card for the GoPro camera and on the Microsoft tablet for the Gigahertz spectroradiometer and Intel depth camera_
2.  Complete all metadata entries on the Excel file After each measurement block.
    a. Hold the cellphone with the compass app horizontally aligned with the GoPro and read out the direction the setup is facing (in degrees), the elevation (in m) and the position in coordinates (add them to the metadata).
    b. Read out the temperature and humidity from the Testo device.

### Post-measurement procedures

1.  After finishing the last measurement block, close all software. Check the saved files on the Document folder in the Microsoft tablet.
2.  Turn off the Gigahertz spectroradiometer by holding a finger on the touch screen for 2 minutes.
3.  Dismount the GoPro, depth camera and spectroradiometer from the holder.
4.  Adding all relevant information to the metadata datasheets.
5.  Connect the GoPro's microSD card to the tablet and copy all files with `.GPR`, `.mp4` and `.jpg` extensions and save them in the `GoPro` folder.
6.  Copy and structure files based on the folder structure as an example folder. Do not rename the files; just copy them to the correct folders and delete any duplicated or mistaken files.
7.  Make a copy of the structured measurement folder on the hard drive.
