# Freebox_OS Plugin

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />

## Changelog Info

### Important

> **_Please note_**: If there is no information about the update, it means that the update consists solely of documentation updates, translations, or minor bug fixes.
>
> **Note: You must have Freebox Server version 4.8.18 for the plugin to work.**

### News Feed

> [View the plugin's news feed on Community](https://community.jeedom.com/t/info-plugin-Freebox-mise-a-jour-des-composants-de-la-delta-tiles-systeme/30673)

## 2026

### 27/04/2026

- Log improvement (Removed line breaks)

### 23/03/2026

- **Phone**
- Added a command for voice messages

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**

### 21/03/2026

- Improvement log

- **Phone**
- Fix call counter (rewind)

- **Home Automation**
- Fix warning in the home automation section if the device does not exist

### 22/02/2026

- Fix the call meter

### 01/02/2026

- Added information to the logs regarding the configuration of slider commands of type slider if the maximum and minimum values are not specified
- Fixed maximum and minimum values for slider-type action commands
- Improvements to the logs for the "titles" section

### 02/01/2026

- USB port on VMs
- Improvements to error messages

## 2025

### 31/10/2025

- Log Improvement for the Disk Search Feature

### 08/10/2025

- Correction to the equipment group for the home automation section

### 04/10/2025

- PHP Warning Correction

### 19/09/2025

- **Wi-Fi**
- Add a list of devices connected via Wi-Fi

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**


### 12/08/2025

- **Global**
- Fix for Cron, which changes every time devices are searched for
- Migration of the mini API to v14

- **VM**
- VM query correction (too many / in the query)
- Fixed the issue with VM equipment being disabled
- Correction action "Stop" - "Restart" - "Start"

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**
>
> **If the scan isn't performed, you may see the following message:** The API version is not compatible ───▶︎ Error Code = invalid_api_version

### 15/07/2025

- Handling the "Nodev" error in Debug mode only (MAC address not found)
- Managing bridge mode to prevent certain information from being retrieved from the player

### 12/07/2025

- **Global**
- Improvements to data retrieval
- Bug Fix: Default Variable During Plugin Update or Installation
- Handling Freebox error messages

- **Network Management**
- Rewrite of the update and device action Network management
- Added information about DHCP

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**

- **List of devices**
- Bug fix: List of network devices

- **LCD Display**
- Display: Option to turn off the LED for compatible devices

- **Freeplugs**
- Bug Fix: Freeplug Data Recovery

- **Parental Controls**
- Improvements to Parental Controls

- **System**
- System-related improvements and updates

- **Wi-Fi**
- Improved Wi-Fi status feedback

- **Player**
- Player Improvements (clean code + no commands created if the variable does not exist)

### 06/05/2025

- API fix not available for Players [Community thread](https://community.jeedom.com/t/freebox-os-messages-derreur-depuis-la-derniere-mise-a-niveau/140390?u=jag)
- Fix for error message regarding unavailable 4G modules [Community Thread](https://community.jeedom.com/t/error-message-inconnue-noent/140388?u=jag)

> **NOTE: The plugin no longer reports communication issues between Jeedom and the Freebox**
> **NOTE: LATEST VERSION OF THE PLUGIN COMPATIBLE WITH DEBIAN 10**

### 05/05/2025

- Fixed an error with PHP <8 [Community thread](https://community.jeedom.com/t/call-to-undefined-function-str-contains/140353/9)

> **NOTE: LATEST VERSION OF THE PLUGIN COMPATIBLE WITH DEBIAN 10**

### 12/08/2025

- **Global**
- Fix for Cron, which changes every time devices are searched for
- Migration of the mini API to v14

- **VM**
- VM query correction (too many / in the query)
- Fixed the issue with VM equipment being disabled
- Correction action "Stop" - "Restart" - "Start"

### 04/05/2025

- **Player**
- Add a command to launch the channels
- Improved button layout on the dashboard
- Improvements and Updates to Commands
- PHP Warning Correction and Bugs
- Improvements to command creation
- Add the date the last time the player was seen on the network
- Added Mute (sound) feature
- Update: Change the volume
- Add channel number information
- Update: Channel name
- Adding the IPv4 address to the player's settings
- Add multiple commands:
      - Open the "Replay" menu
      - Open the "Radio" menu
      - Open Netflix, Prime Video, YouTube, My Recordings
      - Turn on the player with the last channel that was open
- Option to restart the player

> [Thanks to this site](https://github.com/Aymkdn/assistant-freebox-cloud/wiki/Player-API)
> [Thanks to this issue](https://github.com/JEALG/Jeedom-Freebox_OS/issues/446)
> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**
> **New commands are created only if the player is reachable**
**It is essential that the Player be powered on and not in hibernation mode (Révolution) during the search**

- **Smart devices**
- PHP warning correction

- **Freeplugs**
- Added information about Freeplugs

- **Windows and Mac Sharing**
- Adding information to Windows-Mac Sharing

- **Global**
- Improvement, update, and request regarding the Freebox
- Improvements to Request Error Feedback

> [Thanks to this issue](https://github.com/JEALG/Jeedom-Freebox_OS/issues/446)

## 09/02/2025

- Improvements to logs and messages for the cron error "Adding new commands" for connected devices

## 06/02/2025

- Icon name change for the documentation

## 29/01/2025

- API version correction in case of a reset: Upgrade from V10 to v13
- Fix for the "Start Authentication" button
- Plugin repository change > [See GITHUB](https://github.com/JEALG/Jeedom-Freebox_OS)
- Plugin Icon Change

## 28/01/2025

- Migration of the mini API to v13.

### 27/01/2025

- **Wi-Fi**
- Added "Select Scheduled Sleep Mode" command for Wi-Fi on routers compatible with Eco Wi-Fi mode

- **Community**
- Add additional information for Community

- **Scan standard equipment**
- Fix for creating VM-type devices on incompatible Freeboxes

> [View this topic on the community](https://community.jeedom.com/t/api-non-compatible-avec-les-vm-sur-les-freebox-revolution/137141?u=jag)

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**

### 26/01/2025

- Updating documentation links

- **Wi-Fi**
- Added Wi-Fi Eco Mode Mode (for compatible Freeboxes)
- Update the names of the commands in the Wi-Fi map status (in some cases, you may need to run the search twice)
- WPS Status Feedback Correction

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**

### 01/01/2025

- Bug fixes log

## 2024

### 23/12/2024

- **Standard Equipment Package**
- Added check to verify if a disk is present
- Added a check to see if the box is compatible with VMs
- Added a check to verify whether the set-top box is compatible with the various display types on the set-top box screen

- **System**
- Add disk status to system hardware

- **LCD Display**
- Correction: "off" command for orientation
- Fix for the "Screen Brightness" command
- Added support for Freebox Ultra Edition 25
- Correcting the text position value for the display

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD DEVICES**

### 13/11/2024

- Fixed an issue with the Player command creation (you must restart a search to see the status again)
- Fix for Wi-Fi command creation

### 12/11/2024

- Improvement log

- **Phone**
- Added commands for only new missed and received calls
- Bug fix if the list is empty
- Translation correction

### 11/11/2024

- Fix disk creation
- Correct the query for the phone

### 10/11/2024

- Fixed a bug with the authentication launch button
- Type of device grouping correction for flow rates
- Daemon fix: It will only be restarted if authentication was performed during the initial installation.

### 27/09/2024

- Fixed a bug with installation from the Market

### September 25 and 26, 2024

- Translation
- Firmware added to the community link
- Clean code
- PHP 8 Fix
- Translation
- Core mini 4.2
- Bug fix for resetting the phone system
- Function processing Deprecated
- Bug fix for setConfiguration when creating commands

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD AND PARENTAL CONTROL DEVICES**

### 23/08/2024

- Authentication bug fix

### 21/08/2024

> **NOTE: YOU MUST RUN A NEW SEARCH FOR STANDARD AND PARENTAL CONTROL DEVICES**

- **Standard Equipment Package**

- All updates have been applied
- Info Update for Community Regarding Core 4.4
- PHP 8 Warning Fix

- **Parental Controls**

- Add command for "associated device"
- Added command for "Profile-Associated Vacations"

> **NOTE: You will need to delete the ETAT command and rename ETAT(1) to ETAT**

- **Display**

- Added commands to force orientation
- Added commands to hide the Wi-Fi key

- **System**

- Added an information command regarding the Freebox Server firmware update with the following values
      - The update process is initializing
      - The firmware is currently being updated
      - The firmware is up to date
      - An error occurred during the update
- Add display language information

- **Wi-Fi**
- Added information about the Eco type of Wi-Fi mode
- Added sleep mode for Wi-Fi scheduling

### 18/07/2024

- Improvement log
- PHP 8 Warning Fix

### 11/04/2024

- Bug fix during migration from the DELTA box to the ULTRA box

### 10/04/2024

- **General**

- Cleaning up obsolete commands during installation when migrating set-top boxes (Revolution to ULTRA, DELTA to ULTRA).
- LOG Improvements for 4.4

- **Management**

- Improvement Log

- **Wi-Fi**

- Improvements to the Wi-Fi widget to account for power-saving mode (ULTRA Box).

- **VM/PARENTAL CONTROL/Disk**

- If the device (of type VM or Parental Controls) is not detected on the Freebox, it will not be updated and will be deactivated.

- **Records**

  - If no disk is present, the device will not be updated and will be disabled.

- **Tiles**

  - If the box is no longer compatible with this feature:
      - Turning Off the Equipment
      - Removing GLOBAL CRON titles



### 15/02/2024

- Bug fix when deleting the plugin

### 13/02/2024

- Migration of the mini API to v10.

- **Freebox Ultra compatibility begins**
  
  - For the home automation portion: no device updates if migrating from Freebox Delta to Ultra


### 05/02/2024

- Removal of Community link following Core 4.4 update
- Search bar improvements

### 15/01/2024

- Binary inversion correction

### 14/01/2024

- Improvements for Core V4.4

### 06/01/2024

- Improvements to equipment creation **Network Management**
- Second fix for the motion sensor

### 05/01/2024

- Player Update Improvements
- Added Mini4K/POP Player  **Note: No status feedback for this player**
- Equipment is not updated during creation (makes creation faster)
- Typo log
- Display correction for motion sensors

### 03/01/2024

- Player Update Improvements

### 01/01/2024

- Improvements to the Player's information retrieval capabilities for the revolution

## 2023

### 17/12/2023

- Info Update for Community Regarding Core 4.4
- Equipment Improvements for Core 4.4
- Resume, Create, Command, Download
- Resume System Command Creation
- Correction: Undefined variable
- Removal of obsolete commands

- **Tiles**
  
  - Improving the value management of the alarm remote control
  - Alarm remote control button—the button's value is always repeated
  - Log Tiles Improvements
  - Bug fix: Update of info-type commands for the TITLES section
  - Improved handling of binary command inversion for the TITLES section (using the Core's inversion command)

    > **NOTE: YOU MUST RUN A NEW SEARCH FOR TITLES**

- **Smart devices**
  
  - IP4 bug fix for disabled devices
  - Add the IP4 if the device has a static IP address

- **Data Rate**

  - Add transaction details (Received and Sent)


### 04/03/2023

- Undefined variable error
- Typo correction for the Market

### 10/02/2023

- **General**

    > - The API now uses a default variable for all boxes
    > - Modify the non-variable cache to use the Core format "pluginid::custom_key"

- **Tiles**

    > - Bug fix for device registration when global Cron is active

- **Freebox Player**

    > - Bug Fix: Device Status
    > - Added information to the log to distinguish between players
    > - Remove refresh after adding devices

- **Freeplug**

    > - Correcting the equipment type

- **Health**

    > - Add a warning if DEMON is NOK
    > - Add a warning if the device is disabled

- **Phone**

    > - Changes to the "Clear Call Log" and "Mark All as Read" functions

- **Freebox Speeds**

    > - Migration to the new API for 4G/xDSL aggregation.

## 2022

### 27/11/2022

- **General**

  > - Option to reset the API version to v9 without having run the test

### 24/11/2022

- **General**

  > - The API now defaults to v9 for all boxes (it is compatible with the Freebox Revolution)
  > - Added the request path to the message "API NOT COMPATIBLE: Unknown API version"

### 02/11/2022

- **Smart devices**

  > - Bug fix in the port redirection modal

### 29/10/2022

- **Parental Controls**

  > - Fixed the "API NOT COMPATIBLE: Unknown API version" error during an action

### 27/10/2022

- **Wi-Fi**

  > - Bug Fix: Wi-Fi Card Status
  
### 26/10/2022

- **Jeedom Mini Core Version**

  > - Latest version compatible with Core 4.0

- **General**

  > - Stopping active Cron jobs during refreshToken
  > - Set up a weekly Cron job to check for a valid API version
  > - Use of the latest version of the API, which is compatible with all devices
  > - Added a button to the “Pairing” modal to check the API version
  > - Core V4.3 Feature Addition

- **Airmedia**

  > **For all of the new items listed below, you must run the "Scan Standard Devices" scan**

    > Complete rewrite of this section
    > The old commands will be removed because they are incompatible

- **Pairing** (September 21, 2022, September 22, 2022)
  
  > - Added a button to skip the permission check
  > - Added a button to reset the Freebox API

- **Connected Devices** (August 28, 2022)

  > - Correcting the order of devices (connected devices first, followed by unconnected devices)
  > - Rewrite of the refresh command and creation of commands in preparation for future enhancements
  > - The following commands will be removed in the next update because they are now integrated into network management:

    > "Add or Remove Static IP"
    > "Wake on LAN"

- **Network Management**

  > **For all of the new items listed below, you must run the "Scan Standard Devices" scan**

  - New equipment
  - It combines several commands shared across multiple devices

  > - Manage MAC filtering for Wi-Fi
  > - "Add or Remove a Static IP" for devices

- **Parental Controls** (August 17, 2022)
  
  > - Fixed a bug related to searching for new controls

- **Network**

  > - Fixed port reading
  > - Fix: Add MAC address to blacklist or whitelist

- **Tiles**

  > - Add informational text for the global update of titles in the case of SOMFY shutters
  > - Fixed equipment refresh if the global Cron job is not active

- **Wi-Fi**

  > The "Add - Remove MAC Filtering" command will be removed in the next update because it is now integrated into network management

### 30/04/2022

> - Editing the Call List
> - Added information about hard drives
> - Delete Daily Cron Job
> - Option to disable Network command updates (We do not recommend doing this, as it may cause problems in the event of duplicate commands)
> - Delete Daily Cron Job

  > - A specific Cron job can be configured for devices of the "Disk," "Connected Devices," and "Homeadapter" types
  > - If the "Add new commands" field is left blank, the new commands will not be added

### 17/03/2022

> - Modify Homeadapter Command Creation
> - Freeplug Group Bug Fix
> - Added ON/OFF command => Home Adapter, but awaiting a response from Free
> - Modification to Network search with updated device names
> - Update: Create Network Command
> - Correcting VM names during creation

## 2021 

### 06/12/2021

> - Renaming the image folder to meet the new Core requirements
> - Fixed an issue with variables being cleared from the cache
> - Improvements to camera equipment design
> - Bug fix for the ON and OFF commands in the "Titles" section
> - Add Freeplug,

  > - Info: What Freeplug Does
  > - Reset Action
  >   **For all of the new items listed below, you must run a standard device scan**
  >   To use the FreePlugs, they must be paired

### 04/08/2021

- Bug fix for alarm refresh

### 29/07/2021

- Bug fix for VM commands
- Airmedia Correction
- Improvements for Core 4.2

### 27/06/2021

- **Freebox Speeds**

  > - Fix for the fiber-optic data refresh issue on Freebox Revolution devices

- **Downloads**

  > - Fixed an issue with the download mode commands
    > **Old commands will be removed during the update; you’ll need to run the Standard Equipment Scan to get the new command**

### 28/05/2021

- Fixed an issue where Cron stopped and did not restart during a token refresh
- Change the value of the alarm's "Error" command if its value is zero
- Improvements to the search for connected devices

### 23/05/2021

- Fix for Slider Reversal Behavior
- Fixed the ON and OFF commands for all Wi-Fi commands
- Correction: Template Network (Mobile Version)
- Improvements to Wi-Fi WPS Command

### 10/05/2021

- Action: Parental Controls
- Improvements to action tiles (boolean type)

### 08/05/2021

- Fix Reset Pairing

### 07/05/2021

- Improvements to device creation (duplicate management)
- Improvements to the equipment list
- Bug fixes for creating system devices on the Freebox Revolution
- Bridge Mode: The following devices are not created

  > - Air Media
  > - Smart devices
  > - Wi-Fi-Connected Devices (Guest)
  > - Downloads
  > - Wi-Fi

- **Cron/DEMON Improvements**

  - Demon Upgrade
  - Added Cron jobs for actions to compensate for the Freebox's slowness (thanks @Nebz and @Foulek57)
  - Improvement to Cron Refresh Token

- **Improvements Following the Freebox 4.3 Firmware Update**

- **Parental Controls**

  > - Update to Permission Checks During Pairing

- **System**

 > - Add Freebox Language Information

- **Smart devices**

  > - Support for new types of devices (connected vehicles)

- **VM**

  > - Add device (Status, Start, Stop, Restart, and other information)

- **Windows/Mac Sharing**

  > - Option to enable SMBv2
      > If SMBv2 is active, printer sharing commands will be removed during the next device update.
      >
      > Please note: if you enable this feature, Jeedom backups may no longer work if you back up to the Freebox

- **Tiles**

  > - Added a global Cron refresh for the home automation section (thanks @Nebz and @Foulek57)
  > - Bug fix for camera creation
    > **Note: Cameras may be created twice in the Camera plugin**
  > - Bug Fix: Creating Outlets
  > - Added icons for devices (thanks @Skillix)
  > - Improved management of different types of shutters

  > - Added a toggle for certain types of shutters
  > - Bug fix for reversed digital commands
  > [View the plugin's news feed on Community](https://community.jeedom.com/t/info-plugin-Freebox-mise-a-jour-des-composants-de-la-delta-tiles-systeme/30673/54?u=jag)

> **To detect all of the new devices listed above, you must run all the scans**

### 16/02/2021

- Added a "Debug" menu for routers that support Tiles (Freebox Delta)

### 14/02/2021

- Core v4.2 (beta) dashboard display
- Fix for Parental Controls Search

- **Standard equipment**

  > - Add "LCD Display" device—only for Freebox Revolution models
    > **For all of the new items listed below, you must run a standard device scan**

- **Tiles**

  - **HomeAdapter**

    - Improvements to command updates
    - Bug fix for creating commands

  - **Health Page**
    - Display Enhancement
    - Fixed a bug related to battery levels for alarm remote controls

### 23/01/2021

- **Tiles**

  > **To view all the new items listed below, you must run a Tiles Scan**

  - **Alarm**

    - Bug Fix: Status Updates Not Refreshing for Homebridge

### 22/01/2021

- Improved search functionality for additional device commands
- Improved mobile display for the authentication section

- **Smart devices**

  - Added a command to assign a **_static IP address_** from a scenario
    > You need to **search for additional devices** to get the new commands

- **Tiles**

  > **To view all the new items listed below, you must run a Tiles Scan**

  - **Camera**

    - Add this device to the plugin with the ability to:
      - Enable / Disable:

        > - Motion Detection
        > - Activate with the Alarm
        > - HD quality
        > - Flip vertically
        > - Timestamp
        > - Noise Detection
        > - RTSP stream

      - Set:

        > - Sensitivity
        > - Threshold
        > - Microphone sensitivity
        > - Microphone volume

    - The camera is automatically added to the camera plugin if it is installed

      > - Bug fix related to camera creation in the CAMERA plugin

  - **Remote Control**

    - Add battery type to the device
    - Added feature: Turned on the device

  - **Motion/Open Sensor**

    - Added features:
      - Enable / Disable for:

        > - Timer Zone
        > - Main Alarm
        > - Secondary alarm

    - Reversing the state of motion detectors to ensure compatibility with Homebridge
    - Add battery type to the device

  - **Alarm**

    - Added features:
      - Set:

        > - Beep Volume
        > - Siren power
        > - Delay before arming
        > - Delay with siren
        > - Siren duration

    - Improvement to the non-functional Alarm feature with Homebridge

      > - **You must back up the alarm system equipment to receive the upgrades**
      > - **Without this backup, the Homebridge system will no longer work**

    - Add battery type to the device

## 2020

### 13/12/2020

- Bug Fix for Searching for Flow Rate Devices

### 09/12/2020

- Bug fix for alarm not working with Homebridge
  > You need to run another search for the Tiles to resolve this issue

### 08/12/2020

- **Smart devices**

  - Added a command to initiate a **_search for new devices_** from a scenario
  - Added a command to trigger **_Wake on LAN_**; this feature is available via a scenario (in response to a request from @mguyard)

    > You need to **search for additional devices** to get the new commands

- **Wi-Fi**

  - Wi-Fi status feedback fix
  - Add status for the various Wi-Fi cards

- **General**

  - Fix for the search button on system devices

### 29/11/2020

- **Wi-Fi**

  - Added support for managing MAC filtering
  - Ability to add or remove MAC addresses in MAC filtering management from within a scenario
  - Added MAC address filtering: whitelists / blacklists (this filtering is done on a per-scenario basis)

  > You need to **search for additional devices** to get the new commands

- **Smart devices**

  - Added a command to initiate a **_search for new devices_** from a scenario
  - Added a command to trigger **_Wake on LAN_**; this feature is available via a scenario (in response to a request from @mguyard)

    > You need to **search for additional devices** to get the new commands

- **General**

  - Optimizing Equipment Creation
  - General improvements to the display based on the Jeedom template
  - Added tooltips for commands

### 06/11/2020

- Improvements to the list of parent objects
- Added a "Health" page for devices
  > Please note: The battery is not supported for certain devices (remote control, motion detector).

### 28/10/2020

- Fixed the 4G status refresh
- Tile Improvements

### 15/10/2020

> **Thank you**
> Thanks to the beta testers—ipapy, Tom's, Olive, Jcamus86, and Noodom—for their help and feedback

- **Hard Drive**

  - Rewrite this section to support disks with partitions

- **Wi-Fi**

  - Add Wi-Fi WPS command
    > You need to **search for additional devices** to get the new commands

- **Tiles**

  - Bug fix for creating commands

- **Optimization**

  - Taking device versions into account when updating the plugin
  - Log improvement: close session

### 14/10/2020

> **Thank you**
> Thanks to the beta testers—ipapy, Tom's, Olive, Jcamus86, and Freetronic—for their help and feedback
>
> Thanks to Mips for helping to optimize the code to prevent error messages

- **Hard Drive**

  - Incorporation of improvements by @mid.sebastien

  > **Please note: You must modify the configuration of each device**

<p><img src="../images/changelog_disque.png" alt="Disk" width="450" /></p>

- **Optimization**

  - Freebox Débit: Optimizing the Number of Requests
  - Token refresh improvement to accommodate the new Freebox firmware
  - Fixes for undefined variables in the Tiles section
  - Corrections to zero values
  - Cron
    - Cron jobs will not run if the device is disabled
    - Add an additional log entry in case of a problem with a Cron job

### 01/10/2020

> **Thank you**
> Thanks to the beta testers—ipapy, Tom's, Olive, and Jcamus86—for their help and feedback
>
> Thanks to Mips for his help in optimizing the code to prevent error messages

- **System**

  - Add the following information
    - Name: Freebox
    - Feeebox Mode
    - IP
  - Optimization of data retrieval (fewer queries)

- **Smart devices**

  - These features are available only if the Freebox is not in bridge mode
    > For those in bridge mode, you'll need to manually remove both devices from the list of connected devices (Guest Wi-Fi and LAN).
  - Optimizing Refresh and Command Creation
  - Cron Daily: Newly detected devices are invisible

- **Cron**

  - The Cron job will not run if the daemon is _nok_
  - Cron Optimization

- **CronDaily**

  - The Cron job will not run if the daemon is _nok_
  - Cron will not search for connected devices if the Freebox is in bridge mode
    > Don't forget to scan your standard equipment

- **Pairing**

  - Added a link on each window to the plugin's documentation
  - Add a link to the Freebox interface if permissions are not set correctly

- **PHP Optimization**

  - Troubleshooting bugs in info-mode logs
  - Handling Division by Zero

### 12/09/2020

- Option to reverse the numerical values (Action and Info)
- Force removal of the Disk and Network widget
- Removal of 4G data usage (Data is not reported to the API)
- Resolution of the authentication issue following the release of the new Freebox Server firmware version 4.2.5

- **Freebox speeds**

  - Optimizing Data Retrieval

- **Player**

  > You will need to remove the devices after the update.

  > **Status (on or off)**:
  >
  > - The command is created only if the Player returns its status.
  > - It is essential that the Player be powered on and not in hibernation mode. (Révolution)
  > - The Player mini4K is not compatible; the Player POP is not yet compatible

### 30/08/2020

- Bug Fixes: Generic Type Issue with Wi-Fi Scheduling Commands
- Bug Fix: Search for Wi-Fi-Connected Devices (Guest)
- Action on Tiles Controls
- Fixes for inactive color slider
  > You'll need to remove the color slider command and search for the tiles to make this correction.

### 29/08/2020

- **Freebox Speeds**

  - Resuming commands following discrepancies between set-top boxes and protocols
    > Commands will be updated when standard devices are scanned
  - Add ADSL information

- **System**

  - Added the button name to the dashboard for the reboot command

- **Pairing**

  - Add information if the integration of new apps is disabled
  - Changing the progress bar during pairing
  - Add log
  - Adding a message to your Jeedom when a name is missing

- **Downloads**

  - Added connection status information
  - Add schedule status information
  - Added download mode status information
  - Added commands to change the mode type (4 modes)

- **Player**

  - Some players do not return their names. Implementing a workaround to be able to create the device
    > Commands will be updated when standard devices are scanned
  - Add a message to the logs if the Player ID is empty

  ```
  Player : Freebox-Mini-52ec41c5c8d0bbee -- L'Id est vide donc pas de création de l'équipement (mettre sous tension le Player pour résoudre ce problème)
  ```

- **Tiles**

  - Option to reverse the command for slider-type actions
    > You must enter both the minimum and maximum values for this to work

### 26/08/2020

- Fixed a bug causing an infinite loop during the update
- Fixed data speed bug: 4G data speeds are no longer added if the SIM card is not present
- Correcting the Order of Debit Commands

### 25/08/2020

> **Important**
> **You'll need to re-pair the Freebox with the new menu**
>
> **DO NOT PERFORM THE UPDATE IF YOU ARE NOT AT HOME**

> **Thank you**
> Thanks to the beta testers: ipapy, Tom's, Olive, and jcamus86 for their help and feedback
>
> Thank you, Titi_Titi, for helping me improve the plugin

- Improved error messages (if an error occurs, a message is displayed in the message center)
- Removing Widgets That Are No Longer in Use
- Bug fixes for the "refresh" command on certain devices
- Features not available for the box are hidden (e.g., Tile Scan)
- Empty device groups are hidden
- **Daily Cron Job**
  - Added a daily Cron job to check for new connected devices
  - Added a daily Cron job to check for new albums
  - Added a daily Cron job to check for new Home Adapters
- **Pairing**
  - Implementation of a modal type of window to facilitate pairing with the Freebox
    > The menu is now located in the plugin interface
    > The plugin documentation has been updated accordingly [See Documentation](https://mika-nt28.github.io/Documentations/freebox_OS/fr_FR/?theme=light#tocAnchor-1-2-1)
  - Changing the default settings (hiding unnecessary parameters)
  - Added a feature to check permissions; if **NOK**, you cannot proceed (Required permissions are in bold)
  - For the Freebox Delta: You can link the Freebox's rooms to Jeedom devices
  - Option to start searching for various devices after authentication is complete
- **Phone**
  - Removal of all obsolete commands
    > The commands will be removed when the plugin is updated
  - Deleting widgets
  - Resolving line breaks in the call list display
- **Freebox Speeds**
  - Renaming Commands
    > Commands will be updated when standard devices are scanned
  - Added _Ping Response Info_ and _Wake-on-LAN Proxy_
  - Add specific commands for fiber optics (Added only if the _ftth_ module is present)
  - Added specific commands for the _xDSL + 4G_ type of connection
- **Smart devices**
  - Fix for devices not listed in the Freebox not being removed
  - Added a daily Cron job to check for new devices.
  - Option to hide IP addresses on the widget
  - The widget has been renamed
    > You need to **search for additional devices** to get the new widget
- **Downloads**
  - Add RSS feed info
- **Hard Drive**
  - Remove the current widget and use the default Core widget
- **Wi-Fi**
  - Removal of the Wi-Fi On/Off command
    > You must use the ON and OFF commands to manage Wi-Fi
- **Camera**
  - Improvements to Camera Settings
    > You must remove the device to apply the new settings
  - Suppress the camera setup message if the camera is detected
- **Tiles**
  - Fixed a search issue
- **Standard Features**
  - Fixed a search issue
- **Freebox speeds**
  - Added information on IPv4 and IPv6
    > You'll need to search for standard equipment again to get this information
- **Equipment, Wi-Fi-Connected Devices, Guest**
  - Add this device

### 06/08/2020

> Following the Freebox update to version 4.2.3

- Freebox IP Correction

### 29/07/2020

> **Thank you**
> Thanks to the beta testers—ipapy, Tom's, Olive, and jcamus86—for their help and feedback.
>
> Thank you, Titi_Titi, for helping me improve the plugin

> **You must have Freebox Server version 4.2 for the plugin to work**

- Rewrite of the section on creating standard devices
- **Parental Controls**
  - Option to lock or unlock for a selected period of time
    > To take advantage of these new features, you'll need to remove the "Parental Controls" devices and perform a new search
- **All Tiles**
  - Fixes for slider-type shutter commands
- **Download**
  - Corrected the number of downloads; the value was always empty
- **Disk**
  - Improved naming when creating a device
  - Fixed the issue where disk capacity was not updated
- **All equipment**
  - Assignment of different refresh times (Cron) depending on the type of equipment.
    > This will apply only to new equipment

### 24/07/2020

> **Please note: You must have Freebox Server version 4.2 for the plugin to work**
>
> **You'll also need to update the permissions in the Freebox console**
>
> Note: The "Enable/Disable Wi-Fi" command will be removed in future updates; you will need to use the ON and OFF commands to manage Wi-Fi

> **Thank you**
> Thanks to the beta testers: ipapy, Tom's, Olive, and jcamus86 for their help and feedback
>
> Thank you, Titi_Titi, for helping me improve the plugin

- Cleanup: Creating Commands
- Added an icon for batteries
- Migration of all APIs to V8
- Rewrite the "update" and "refresh" sections
- Creating a class template, and refreshing and updating
- Cleaning APIs
- Creating the Freebox_OS.inc class
- Bug fix for creating disk commands
- **Renaming devices**
  - _ADSL_ becomes _Freebox Débits_
  - _AirPlay_ becomes _Air Media_
  - _Network_ becomes _Connected Devices_
- **Alarm**
  - Bug Fix for Freebox Alarm Widget
  - Added names and icons for modes
  - Creating specific commands to integrate it into Homebridge

    > - We strongly recommend removing this equipment to receive the new commands

- **Alarm Remote Control**
  - Retrieve the latest status
- **System**
  - Reporting of New Status Updates
    > We recommend removing the device and searching for standard devices.
- **4G**
  - Added a command to enable/disable 4G on the router
    > Commands are added only if the card is detected
- **Wi-Fi**
  - Add Schedule => Status + Enable + Disable
  - Added a generic device type for Wi-Fi (to command it via Homebridge)
- **Parental Controls**
  - Add parental controls => Status
  - Added "unlock" and "lock" commands (30 min/1 hr/2 hrs)
- **Camera**
  - Update to manufacturer and model information following integration into the Camera plugin
- **Smart devices**
  - Widget support for new device images
  - Fixed bugs related to the handling of empty ports
- **All Tiles**
  - Bug fixes for lighting sliders of different types
    > You must delete the commands to resolve this issue.

### 05/07/2020

- Fixed bug related to transparency of network equipment and disks
- Bug Fix: HomeAdapter Status
- Compatibility with V3 for certain icons
- Align alarm command icons based on the Alarm plugin
- **Camera**
  - Add a log entry upon creation
  - Modify the camera settings when creating the device in the **_Camera Plugin_**; this will allow for better integration with Homebridge.
    > Please note that the settings on the existing equipment have not been changed.
    >
    > - Either remove the device and run another scan of the Tiles
    > - Change the following settings:
    >   - **Feed URL**: rtsp://#username#:#password#@#ip#/img/live
    >   - **Video frames per second** _(Capture tab)_: 15

### 02/07/2020

- **Wi-Fi**
  - Routing commands to a specific Wi-Fi device
    > Please note that this feature is disabled by default
  - Added icons for the ON and OFF commands
  - Added a widget for Wi-Fi status and on/off action (V4 only)
  - Migration from API Version 3 to Version 5
- **Phone**
  - Widget Improvements
  - Added icons for the various commands (in color for V4)
- **Download**
  - Added icons for the various commands (in color for V4)
  - Assigning Core Widgets to Different Commands
- **Systems**
  - Added icons for temperature and the fan
  - Added icons for the "Update" and "Reboot" buttons (in color for V4)
  - Corrections to the equipment type
  - Update of the minimum and maximum values for certain commands
- **AirPlay**
  - Added stop and play icons (For new installations only; in color for V4)
- **Tiles**
  - Brightness bug 0 to 255 + min/max display on digital commands
  - Add Switch/Toggle-type BP type
  - Linking actions and commands for blinds and lighting types
  - Moving the "Search for Homeadapter" function to the Tiles search (Required only for Freebox DELTA)
  - Combining the Tiles and Homeadapter features
  - Improvements to the alarm widget
  - Add information about the action type and device
    > You need to click "Scan Tiles" to get this information
- **Corrections and Improvements**
  - Bug Fix: **Stepper motor loops when the plugin is activated**
  - Disable device creation during initial setup
  - Added a command to search for Freebox system devices
  - Add network analysis after searching for system devices
  - Added to the list of commands: icon, min-max
  - Disable device creation during initial setup
    > You'll need to click "Scan standard devices"

### 11/06/2020

- Bug: Battery Display Fix: Hidden by Default
- Bug: Default template for tampering and opening
- Bug: Default value reversed on the cover + template assignment
- Bug: Presence sensor—template corrections and signal reversal
- Permission to delete commands

### 09/06/2020

- Change to battery alarm notification when creating the command

### June 7 and 8, 2020

- "Tiles"-type devices

  - Assigning Tiles to Categories (Security, Lighting)
  - Fixed ON/OFF button bug \* Added information to the log in debug mode
  - Replace ' in the name of the device or command with a space
  - Replace "É" with "E" in command names
    - Hiding the "Add Command" button
    - Added generic types to certain commands
    - Changing the default visibility of certain commands (Battery, PIN Code => hidden)
    - Fixed an issue where the "Search" command did not appear in the "Home Adapter" device after an initial search \* Renamed commands (added "Status" when the command and the information have the same name)
      > To see all the new device updates, you need to clear them and then click "Search for Tiles."

- Added "refresh" command => command hidden by default in the command lists
- Clean code

### 27/05/2020

- Add information when searching for Tiles
- Improved command display
- Migration of Wi-Fi commands from V3 to V5
- Separation of Home and Tiles devices in the device list
- Cleaning Up Cron Jobs When Deleting the Plugin

### 03/04/2020

- Separation of the plugin and its documentation

## 2019

### 19/12/2019

- Bug Fix: Syntax Error

### 11/12/2019

- Bug fix: Disconnection in case of an incorrect response
- Removing network devices in the event of an invalid response

### 10/12/2019

- Restructuring of the API class
- Creating a cron job to refresh the token so that there is only one session
- Network Widget Update

### 27/11/2019

- Adding widgets for the mobile version
