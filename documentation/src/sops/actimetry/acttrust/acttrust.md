# Standard operating procedure for ActTrust2



**Act Studio SOPs**

For the description below, the ActTrust software (ActStudio) version used was: v.1.0.23
The most up to date version is v.1.0.24



**Setting up a recording**

1. Open ActStudio
2. Connect your ActTrust with the computer (via cable and docking station)
3. (Potentially need to “power up” the device with the green button at the right bottom)
    
    ![ActStudio-window.png](img/ActStudio-window.png)
    
4. Change the name of the Participant ID under “Trial information” > name
    -> There are cases in which the Participant ID does not need to be specified, e.g. when there is no participant wearing the device in environmental measurements. In those cases, it would be recommended to use an identifier that is specific to the project.
5. Note down the device number and link it with the participant ID
6. Do not enter any additional information, e.g. gender or date of birth
7. Leave the description free unless absolutely necessary
8. View “Desired” and “Current” configurations to determine whether a change needs to be made in mode, intervals, threshold and UV sensor data collection
9. Change the default preferences by going to “configurations” at the bottom of the page > click on preferences
10. A new window appears: set the default preferences as discussed and click apply  
    1. Note: The specific settings from acquisition are project-dependent and there is a trade-off between memory capacity and sampling. For most projects <1 month, 30 sec intervals are appropriate.
11. Default settings:
    
    ![2022.12.15.Screenshot_14.30.52.png](img/2022.12.15.Screenshot_14.30.52.png)
    
    ![2022.12.15.Screenshot_14.31.13.png](img/2022.12.15.Screenshot_14.31.13.png)
    
    ![2022.12.15.Screenshot_14.31.28.png](img/2022.12.15.Screenshot_14.31.28.png)
    
    ![2022.12.15.Screenshot_14.31.44.png](img/2022.12.15.Screenshot_14.31.44.png)
    
    ![2022.12.15.Screenshot_14.31.51.png](img/2022.12.15.Screenshot_14.31.51.png)
    
    ![2022.12.15.Screenshot_14.41.10.png](img/2022.12.15.Screenshot_14.41.10.png)
    
12. Check the battery status and charge if necessary (wait until battery status turned green and says “charged”)
13. Check if the system clock and the device clock are synchronised
14. Now click “Start Trial” 
15. Check at the bottom under “configurations” if the “desired” settings are similar to the “current” settings
    
###*After disconnecting*
    
1. Note down in the Actimetry database that it was taken
2. After the study, immediately connect the ActTrust so it stops recording
    
    
**Data readout and download**
    
1. Place ActTrust device into the docking station and connect cable to laptop/computer
2. Open ActStudio
3. Check whether the device is connected
        
        ![Screenshot 2023-01-19 at 16.33.13.png](img/Screenshot_2023-01-19_at_16.33.13.png)
        
4. Check the clock difference from the device and the internal time of your machine under “system” vs “device” on the right side > note this down!
5. Click “Finish Trial” > this loads the data
6. Wait until 100% is downloaded (check the progress bar)
7. In some cases: Possible a warning message appears which asks you whether you want to fill gaps in the data with 0s -> “Do nothing” to preserve missing periods of data (rather than imputing with 0). In a later analysis stage, this can be revisited and ActStudio will prompt you again.
        
        ![Screenshot 2023-01-19 at 16.57.08.png](img/Screenshot_2023-01-19_at_16.57.08.png)
        
8. A new window opens > specify the file name and the path where to save it; this saves the raw data
        
        ![Screenshot 2023-01-19 at 16.36.55.png](img/Screenshot_2023-01-19_at_16.36.55.png)
        
9. Another window opens: “Please attention: Do you want to add the data to the log” > Click “Yes”. This stores the data in the local data base and you can always open it again without the need to upload the raw data file again
        
        ![Screenshot 2023-01-19 at 16.58.28.png](img/Screenshot_2023-01-19_at_16.58.28.png)
        
10. Do NOT crop the data to valid periods in ActStudio by setting the initial and final times. Rather, this should be done with a separate file (start stop log file) to be loaded in pyActigraphy for example.
    
    **Visual inspection of data**
    
11. Click on “Calculate Analysis”. This will generate metrics based on the data. This only has to be done once and the analyses will be available under “Analysis”.
12. Under “Analysis”, a lot of different data are depicted in line plots. For the initial visual inspection, it is sufficient to select “Activity”, “Sleeping”, “Resting”, “OffWrist” and “Light”.
    
    ![Screenshot 2023-02-03 at 10.56.30.png](img/Screenshot_2023-02-03_at_10.56.30.png)
    
13. Periods of “Awake” and “Sleep” will be scored by algorithm by ActStudio. You can change the type of algorithm in settings.
    

##General notes
- View data in ActStudio, either for visual inspection or as a check that the data are there. For quantitative analyses, we will pyActigraphy.
- Decide in advance on how to instruct pariticpants concerning the event button
