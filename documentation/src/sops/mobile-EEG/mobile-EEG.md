# Standard Operating Procedure for Mentalab Explore mobile EEG

| Device       | Mentalab, Mentalab Explore EX8M            |
| ------------ | ------------------------------------------ |
| Objective    | Acquire ambulatory EEG data                |
| Owner        | [Laura Hainke](mailto:laura.hainke@tum.de) |
| Reviewer     |                                            |
| Approver     |                                            |
| Contributors |                                            |
| Version      | 1.0.0                                      |
| Last edit    | [Laura Hainke](mailto:laura.hainke@tum.de) |
| Date         | 29.10.2023                                 |

## Start up

Please refer to the [manufacturer’s website](https://wiki.mentalab.com/user-guide/) for complete information on the product. Note that it describes the newer system version, though most of it also applies to the EX8M model.

### EEG system core components:

- Amplifier: Mentalab Explore EX8M (8 channels, with memory)
- Software: [download for Windows or Ubuntu](https://wiki.mentalab.com/explore-desktop-guide/) (latest version)
- Set of 9 cables (different types available), attached to a connector specific to the amplifier.
- The connector has 10 pins, one of which is empty. The cable inserted into the pin on the opposite side of the connector is the system reference (REF); starting from there, the remaining electrodes are the active channels 1 - 8. This system does not have a ground (GND), since it is not attached to a power line.

### Variant 1: wet EEG

- Cable set: ring gel type electrodes
- Cap (size M, L, or XL)
- Consumables: Ethanol, cotton sticks, abrasive gel, measurement band
- For short measurements: blunt syringe + conductive gel. For long (e.g., overnight) measurements: 10-20 paste

### Variant 2: dry EEG

- Cable set: snap button
- Consumables: Ethanol, cotton sticks, abrasive gel, cotton pads, disposable “stick & peel” electrodes, tape

### How to start the system:

- Connect the amplifier to a power source using a micro USB cable. Charge it fully for up to 3 hours.
- Disconnect the device from the power source and press the button once to turn it on. The device LED should blink once in green, then start blinking in blue, indicating it is ready for Bluetooth pairing.
- On your computer, which must have the software installed and a working Bluetooth module, open the Explore Desktop app.
- Enter the device ID and press Enter. You can find it on the back of the amplifier, it is composed of the last 4 characters on the printed sticker (e.g., 82X9).
- Either a pop-up will appear asking for your permission to establish Bluetooth connection, or you will have to add the device manually in your Bluetooth menu.
- The Explore Desktop app will move to the settings page as soon as the device has established Bluetooth connection.

## Preparation

General rule: communicate with your subject. Some people may complain about EEG setups, e.g., due to skin sensitivity. In that case, be more gentle when cleaning their skin.

### Wet EEG:

- To prepare the cap, take the ring electrode set and thread the cables through the larger cap holes, to limit cable movement. Press the rings into the smaller holes of the cap until fixated. Note that the first electrode of the set is the system reference. Each small hole is marked with an EEG position according to the 10-10 system.
- Put the cap which most closely matches the subject’s head size on their head. Fasten the velcro strap over the chin. It should be as tight as possible, without making the subject too uncomfortable.
- Extend the measuring band from nasion (between the eyebrows) to inion (the base of the bone at the back of the skull). Adjust the cap so that the Cz electrode is in the middle. Then, measure from ear tip to ear tip; adjust the cap so that the Cz electrode is in the middle.
- Insert the cable connector into the amplifier until it clicks (there is a correct up- and downside of the connector). The amplifier can be attached to the cap using a velcro patch, or to any fabric using a clip.
- Preparing electrodes:
  1.  Lift the electrode + surrounding cap fabric slightly. Clean the underlying skin with a cotton stick dipped in Ethanol, then dip it in abrasive gel and scrub the skin, moving some hair away if possible from underneath the electrode.
  2.  If using a syringe and gel, place the blunt tip underneath the electrode and apply gel. If using 10-20 paste, apply some directly onto the inside of the electrode. Press the electrode onto the scalp.
  3.  The gel or paste should fill the electrode and reach the scalp, but not overflow visibly around the electrode.

### Dry EEG:

- “Stick & peel” electrodes only stick to bare skin. If needed, adapt the positions of choice according to the subject’s facial or body hair.
- Clip the electrodes into the snap buttons beforehand.
- Fixate the cables to the skin or to the clothes, to limit cable movement.
- Preparing electrodes:
  1. Clean the position with a cotton stick dipped in Ethanol, then dip it in abrasive gel and scrub the skin carefully. Remove the abrasive gel with a dry cotton pad (else, the electrode may not stick).
  2. Remove the cover of the disposable electrode and press it onto the cleaned location.

### After the setup:

- Go to the impedances tab in the Explore Desktop app. Choose wet or dry in the dropdown, then check the values. Green values are desirable.
- For wet EEG, impedances should be < 10 kOhm, ideally < 5 kOhm. If the value is higher for any electrode, try to clean the spot more thoroughly using some more abrasive gel, and apply more gel/paste.
- For dry EEG, there is no consensus. < 100 kOhm is usually good.
- Go to the signal visualization tab. Ask the subject to lean back and relax. Check if any channel is particularly noisy. If all channels seem noisy, or all impedances are high (in the case of wet EEG), the reference channel requires more thorough preparation.
- Sanity check: ask the subject to blink their eyes a few times, then clench their teeth, then close their eyes. You should be able to see the artifacts and the shift to alpha activity, in most cases.

## Recording Procedure

### Variant A: recording to system memory

- Go to the settings tab. Click on “format memory” to wipe the system memory clean, so the recording contains almost exclusively relevant data. Taking this step deletes the data recorded during setup and impedance measurement.
- Note: The system initializes a new data file and starts recording to the internal memory as soon as it is switched on. The data file will be filled until the device is switched off.
- If desired, change the sampling rate. 250 Hz is the default; 500 Hz or 1000 Hz are possible.
- Close the app and start the experiment. The device will leave Bluetooth mode and move to offline recording only.

### Variant B: recording to PC

- If desired, change the sampling rate. Channel names can also be changed (e.g., from “1” to “Cz”).
- Go to the signal visualization tab. In the pop-up, enter your filter settings; note that they apply only to the visualization, the signal recorded is always the raw data. Press record, enter a folder and filename. Press stop when the trial is over; repeat as needed.
- Important: the Bluetooth range is about 10 m, but Bluetooth interference can easily happen indoors. The higher the sampling rate, the more problematic this will be. Having the subject + system and the recording PC in separate rooms is a bad idea. In general, recording onto the memory is preferable. If inconvenient, test your setup well beforehand.

### How to get good quality data (_depends on the experimental setup_):

- Ask the subject to remain as calm and relaxed as possible. Explain that speaking, moving, teeth clenching, and muscle tension are electric activity, captured by the system on top of brain activity.
- If your experiment is longer than 1 hour and you are using wet EEG, check impedances every 1-2 hours. Apply more paste when needed, as it may dry up. Disposable electrodes usually prevent this issue.
- If the task given to subjects takes more than a few minutes or is not very engaging, make sure to take breaks and keep them alert.

When the experiment is terminated, turn off the amplifier by pressing the button until the LED blinks in red 3x.

## Data Saving

This applies only to variant A; in variant B, the files are already in the folder you specified.

1. Make sure the amplifier has been turned off. The LED should be off. _Connecting the device to a power source while still recording will result in a corrupted data file!_
2. Connect the device to your PC using a micro-USB cable that is appropriate for data transfer. Look for the Explore device in the list of connected external drivers and open the folder.
3. In the folder, you will find one or more files, with the name pattern DATA[3 digits].BIN. If you have cleared the memory beforehand, there should only be one file, named DATA000.BIN. The longer you record, the larger the file will be. If there are multiple files, consider file size and order to determine which one corresponds to your recording period.
   - Example: you’ve turned the device on to check if all is well, then turned it off again. Then, without clearing the internal memory, you have recorded until full capacity was almost reached, then turned it off. Lastly, you turned it on and off again by accident. Result: your folder will contain 3 data files. Only the middle one contains the data you want and will have a size considerably larger than the others.
   - Recommendation: Every time you record a period meaningful for your experiment onto the memory, save the data and clear the memory before starting the next period.

## Terminating

### Resetting the system for the next recording:

- Make sure the device is turned off, then leave it to charge for about 3 hours to fill the battery.
- When turning the device back on, it may blink in pink a few times, before shutting down automatically. This indicates the memory is filled over a certain threshold. To continue, restart the device. If you are sure you have backed up the data, double-click the button during the period of blink flashes; this will wipe the memory clean. If you are unsure, let the device shut down, back up the data, and repeat.

### Cleaning the equipment:

- Wet EEG: Remove the electrodes from the cap. Clean the cap with water and soap, leave it to dry or blow-dry. Clean the electrodes with a brush under running water, being careful not to scratch the inner metal parts. Do not expose the connector to water, it may be damaged over time.
- Dry EEG: Detach the disposable electrodes and throw them away. Disinfect the cables if needed.
