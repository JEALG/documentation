# Freebox_OS plugin

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />


## Description

This plugin allows you to retrieve information from your FreeboxOS (Freebox Revolution, 4K, DELTA, POP, or Ultra server) and interact with it via widgets or scenarios that incorporate the commands you’ve created.

>
> **You must have Freebox Server version 4.12.1 for the plugin to work**

The information available from your Freebox Server on Jeedom is:

- **System Information:**
  - Turn off Wi-Fi
  - Restart your Freebox
  - Internet speeds
  - Your connection status
  - Call Filtering Management
- **Phone:** in the last 24 hours
  - Number of missed calls
  - The number of calls made
  - The number of calls received
  - Number of voice messages
- **Hard Drive:**
  - The available storage space on your hard drives connected to the Freebox Server.
- **Devices connected to the LAN and Guest Wi-Fi:**
  - The status of each DHCP device
  - The **_Wake on LAN_** command can only be used within a scenario
- **Home Automation (DELTA only):**
  - Retrieves information from the smart home

## Installation and Configuration

Once the plugin is installed and active, no configuration is required.

## Pairing (Authentication)

Go to the plugin's main page and click

<p><img src="../images/appairage.png" alt="Pairing Dialog" width="60" /></p>

Next, follow the on-screen prompts to confirm the pairing

<p><img src="../images/freebox_os_screenshot2.png" alt="Authentication 1" width="300" /></p>

### Settings

In the window below, you can modify

- **IP Freebox**: Freebox login address _(default: maFreebox.Freebox.fr)_
- **Name of the connected device**: The name of the Jeedom (this field is locked)
- **Automatically add detected devices to:** : Specify the default room
- You can click the **Reset configuration** button to restore the default settings
  > - Retrieves the **name of your Jeedom** if it has changed since the last pairing
  > - Restores default settings for:
  >     - **Freebox API version**: v10
  >     - **IP Freebox**: maFreebox.Freebox.fr
  >     - Clears other plugin configurations

- Don't forget to click **Save** after making your changes

> It is essential that your Jeedom be named in order to continue pairing the plugin with your Freebox

<p><img src="../images/freebox_os_screenshot3.png" alt="Authentication 2" width="300" /></p>

### Authentication

#### Minimum Freebox firmware version

 > The plugin requires a minimum firmware version to function.
 > The minimum firmware version is listed in the changelog at the beginning and at the start of this documentation

#### Authentication

In the window below, you will be prompted to authenticate on the Freebox

- Click the **Start Authentication** button
- Monitor the login information on both this screen and the Freebox

<p><img src="../images/freebox_os_screenshot4.png" alt="Authentication 3" width="300" /></p>

### Permissions Check

In the window below, the system will check the permissions assigned to the application

- See the "Access Rights" section (in this documentation) to modify the rights on the Freebox
- Once the permissions have been set, click the **Verify Permissions** button.
  > If permissions are OK, the **Next** button will become visible
  > Mandatory rights are in bold

<p><img src="../images/freebox_os_screenshot5.png" alt="Authentication 4" width="300" /></p>

### Link Freebox rooms to Jeedom rooms

> This window appears only if the Freebox is a DELTA
>
> You can enable or disable the "Global Tile Refresh" Cron job
>
> <b>Don't forget</b> to click "Save" to apply the changes

<p><img src="../images/freebox_os_screenshot6.png" alt="Authentication 4" width="300" /></p>

### Scan

In the window below, you can start scanning the various devices.

<p><img src="../images/freebox_os_screenshot7.png" alt="Authentication 5" width="300" /></p>

### Authentication complete

Authentication was successful.

<p><img src="../images/freebox_os_screenshot8.png" alt="Authentication 6" width="300" /></p>

### Authentication problem resolved

If you encounter an authentication issue, you must provide the plugin logs in debug mode
Here is an example
```
000|[2024-10-11 18:53:49] INFO  ──────────▶︎ Étape : setting
0001|[2024-10-11 18:53:49] INFO  ───▶︎ IP : mafreebox.freebox.fr
0002|[2024-10-11 18:53:49] INFO  ───▶︎ Nom API : Plugin Freebox OS
0003|[2024-10-11 18:53:49] INFO  ───▶︎ Id API : plugin.freebox.jeedom
0004|[2024-10-11 18:53:49] INFO  ───▶︎ Nom de votre Jeedom : JAG Jeedom-VM2
0005|[2024-10-11 18:53:49] INFO  ───▶︎ Objet par défaut : 13
0006|[2024-10-11 18:53:49] INFO  ───▶︎ Version API Freebox : v12
0007|[2024-10-11 18:53:51] INFO  ──────────▶︎ Étape : authentification
0008|[2024-10-11 18:53:53] INFO  ──────────▶︎ Étape : rights
0009|[2024-10-11 18:53:57] DEBUG  OK  Close Session
0010|[2024-10-11 18:53:57] DEBUG  [Freebox Close Session] : {"uid":"","success":false,"msg":"Vous devez vous connecter pour accéder à cette fonction","result":{"password_salt":"","challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr"},"error_code":"invalid_session"}
0011|[2024-10-11 18:53:57] DEBUG  [Freebox Password] : {"success":true,"result":{"logged_in":false,"challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr","password_salt":"","password_set":true}}
0012|[2024-10-11 18:53:57] DEBUG  [get Freebox Open Session Data] : {"result":{"session_token":"eRDFtl35L8ENEND2UGlooFzLhAgmv8CGPbMLiegdyC2n4z3DDr4UEYY+zYMOhSkS","challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr","password_salt":"P","permissions":{"parental":true,"contacts":true,"explorer":true,"tv":true,"wdo":true,"downloader":true,"profile":true,"camera":true,"settings":true,"calls":true,"home":true,"pvr":true,"vm":true,"player":true},"password_set":true},"success":true}
0013|[2024-10-11 18:53:57] INFO  ───▶︎ Les droits sont OK
0014|[2024-10-11 18:53:58] INFO  ──────────▶︎ Étape : room
0015|[2024-10-11 18:53:58] INFO  ───▶︎ Cron Global Titles ACTIVATION : NOK
0016|[2024-10-11 18:53:58] INFO  ───▶︎ Compatibilité avec la partie domotique : NOK
0017|[2024-10-11 18:53:58] INFO  ──────────▶︎ Étape : scan
0018|[2024-10-11 18:53:59] INFO  ──────────▶︎ Étape : end
```

<p><img src="../images/debug_log.png" alt="Enable debug log" width="300" /></p>


## Access Rights

Certain additional access rights are required to use the plugin; they **must be assigned and modified** directly from the Freebox's operating system

- Log in to the Freebox interface (http://maFreebox.Freebox.fr)
- Open the Freebox settings

<p><img src="../images/freebox_para.png" alt="Freebox settings" width="100" /></p>

- Open the Freebox access management settings _(this setting is located in Advanced Mode)_

<p><img src="../images/freebox_gestion_acces_1.png" alt="Freebox access management settings" width="600" /></p>

- Click the **Applications** tab
- From the list, select the application specified during plugin installation _(default: Freebox OS plugin)_

<p><img src="../images/freebox_gestion_acces_2.png" alt="Freebox access management settings" width="500" /></p>

- **Grant all access rights**

<p><img src="../images/modification_droit.png" alt="Modifying specific access rights" width="500" /></p>

# Standard Equipment

Click the **_Scan standard devices_** button; the plugin will create the various standard Freebox devices.

<p><img src="../images/recherche_systeme.png" alt="Search for system devices" width="60" /></p>

The following devices and commands will be created:

- **LCD display**
  - Brightness adjustment
  - Adjusting text orientation
  - Hide the Wi-Fi key
  - Light strip control (if the box is compatible)
  - Turn off the LED (if the box is compatible)
- **Air Media**
  - Select Current Player
  - AirMedia Start/Stop
- **Connected Devices** and **Guest Wi-Fi Connected Devices**
  - All devices connected to the Freebox
  - Option to use the **_Wake on LAN_** command (only via a scenario)
- **Hard Drive**
  - Disk usage
  - Temperature
  - RAID type (only for compatible Freebox models)
- **Freebox Speeds**
  - Freebox download speed, upload speed, bandwidth up, bandwidth down
  - Freebox Media
  - Freebox status
  - Connection type
  - Connection Status
  - IP
  - Response to ping
- **Player**
  - Mac
  - Type
  - Model
  - Version
  - API available
  - Available on the network
  - Status (on or off)
    > The command is created only if the Player returns its status and has an ID.
    > **It is essential that the Player be powered on and not in hibernation mode (Révolution) during the search**
    > The mini4K/POP players are available, but they do not report their status
- **Windows-Mac File Sharing**
  - Enable/Disable File Sharing on Mac, Windows, and FTP
  - Enable/Disable Printer Sharing (available only if SMBv2 is not active)
- **System**
  - Update
  - Reboot
  - Freebox firmware version
  - Mac
  - IPv4/IPv6
  - Fan speed
  - Temperatures _(temp sw, temp cpub, temp cpum)_
  - On since
  - board name
  - serial
  - 4G if the SIM card is inserted in the Freebox
- **Phone** over the past 24 hours
  - Number of Missed / Received / Placed Calls
  - List of Missed / Received / Placed Calls
  - Number of voice messages
  - List of Played and New Voice Messages
- **Downloads**
  - Number of tasks
  - Number of active tasks, tasks being retrieved, tasks being repaired, tasks being verified, tasks on hold, tasks with errors, stopped tasks, completed tasks, RSS feeds, and unread RSS feeds
  - Downloading...
  - Receive and transmit speeds
  - Start, Stop
  - Mode de téléchargement
  - Schedule Status
  - Login Status
- **VM** (only for compatible Freeboxes)
  - Status
  - Possible actions: Stop, Restart, Start
  - Info: Number of CPUs, MAC Address, Memory, USB Port, Virtual Display, Disk Type
- **Wi-Fi**
  - Wi-Fi Status
  - Wi-Fi On/Off
  - Call Filtering Management
  - Schedule Status
  - WPS Session ON/OFF
  - Blacklist
  - Mac Whitelist
  - Wi-Fi Map Status

## Parental Controls

Click the **_Parental Controls Scan_** button; the plugin will create the various Freebox system devices.

> These controls were introduced with version 4.2 of the Freebox.

<p><img src="../images/parental_controls.png" alt="Search for parental controls" width="60" /></p>

- The following devices and commands will be created:
  
  > - Status
  > - Block
  > - Allow
  > - Block 30 min/1 hr/2 hrs

## Features of Home Adapters (Freebox Delta only), Connected Devices, Hard Drive, and System

These four devices are empty by default when they are created, except for the system, which includes information common to all Freeboxes.

Open each device and click the "Search" button

> The plugin will search for and create the various associated commands

<p><img src="../images/recherche_commandes.png" alt="Search for specific devices" width="800" /></p>

> A daily Cron job automatically checks for new devices

## Network management

This equipment allows you to:

> - Assign a static IP address
> - Manage MAC address filtering
> - Wake-on-LAN feature
> - Change the device type

### Assign an IP address

<p><img src="../images/modif__equip_ip_fixe.png" alt="Change IP" width="800" /></p>

The following fields must be filled in

- Select the connected device
- Select and modify device with the next value

  > - **Add Static IP**
  > - **Remove Static IP**
  > - **Change the device's IP address**

It's also possible to do this using the command
   > - **Change Device Type / IP**

- IP Selection: Enter the device's IP address
- Device Name Selection: Enter the device name

  > If the name field is empty, the plugin will retrieve the device name entered in the Freebox

- Comments: Allows you to enter a comment (Optional)

### Change the device type

<p><img src="../images/modif__equip_type.png" alt="Editing equipment" width="800" /></p>

The following fields must be filled in

- Select the connected device
- Select and modify device with the next value

  > - **Change Device Type / IP**

- Device Type Selection: Select the device type

  > If the name field is empty, the plugin will retrieve the device name entered in the Freebox
  
- Comments: allows you to enter a comment
- Edit device: Sends the changes to the Freebox

### Manage MAC address filtering (Wi-Fi)

<p><img src="../images/modif__equip_filtrage.png" alt="Modifying equipment" width="800" /></p>

This can be done using commands from connected devices or Wi-Fi-enabled devices
The following fields must be filled in

- Select the connected device
- Select and modify device with the next value

  > - **Add/Edit Blacklist**
  > - **Add/Edit Whitelist**
  > - **Delete Blacklist/Whitelist**

- Comments: Allows you to enter a comment or a password
- Edit device: Sends the changes to the Freebox

### Wake-on-LAN feature

<p><img src="../images/modif__equip_wol.png" alt="Editing equipment" width="800" /></p>

- Select the connected device
- Select and modify device with the next value

  > - **Wake on LAN**

- Comments: Allows you to enter a password
- Edit device: Sends the changes to the Freebox

This is managed via the modal from the connected devices widget or from a scenario.

## Freebox Delta

> The Freebox Delta offers a security package and connectivity with certain devices.

Click the **_Scan Tiles_** button; devices and commands for the various connected devices will be created

<p><img src="../images/recherche_tiles.png" alt="Search for specific Freebox Delta devices" width="60" /></p>

### Alarm Status

> The plugin reports the alarm status via the "Alarm Status" command

![Alarm status](../images/alarme_statut.png)
Possible values are:

> **idle** = Alarm disabled
> **alarm_1_arming** = The main alarm is armed; this is a countdown during which only sensors located outside the zone can trigger the alert
> **alarm_2_arming** = The partial alarm is activated; this is a countdown during which only sensors located outside the zone can trigger the alert
> **alarm_1_armed** = Full alarm activated
> **alarm_2_armed** = Partial alarm armed
> **alarm1_alert_timer** = The main alarm was triggered by a sensor in the time zone, and the siren will sound after a countdown
> **alarm2_alert_timer** = The night alarm was triggered by a sensor in the time zone, and the siren will sound after a countdown
> **alert** = The siren is sounding

> The alarm system is compatible with Homebridge and the mobile app: no configuration is required.
> To enable integration, information commands have been added to allow interaction with the Alarm plugin.
>
> - **Active** = Binary Information (1 = Alarm Activated)
> - **Status** = Binary Info (1 = Siren active)

<p><img src="../images/alarme_dashboard.png" alt="Alarm status" width="250" /></p>

### Remote Control Status

> The plugin tracks the remote control's history and displays the last action performed by the remote control.

- Possible values are:
  > **null** or **0** = No status
  > **1** = Main alarm
  > **2** = Disable
  > **3** = Secondary alarm

### Cameras

> Cameras are created automatically if the camera plugin is installed

## Refresh time (Cron) for devices

- You can modify the refresh schedule for each device; by default:

  > Home Adapter, FREEBOX - Remote Control (Alarm), Parental Controls, and My Devices (excluding hard drive) = **Cron will be set to 5 minutes**
  >
  > Hard Drive = **Cron will be set to 1 hour**

- This Cron job refreshes various information-type commands; the equipment is automatically updated whenever a command is executed.
  > Action commands are not affected by this Cron job.
  >
  > The shorter the time, the greater the load on the Freebox's CPU.

- Starting with plugin version 20210507, for the **home automation section**
  > A global refresh Cron job is enabled by default
  >
  > <p><img src="../images/cron_tiles.png" alt="Refresh time" width="800" /></p>
  >
  > If this option is disabled, **Cron will be set to 1 minute**

## Tiles

*Not all devices are necessarily integrated into the system due to updates to the Freebox*S*

- To integrate the new systems, you must:

  > Set the plugin to debug mode
  > Restart the Daemon
  > Create **_Debug Tiles_**

<p><img src="../images/debug.png" alt="Debug Tiles" width="60" /></p>

Start a thread (if there isn't already one addressing this request) on the community and provide the following information

- Take a screenshot of the equipment

<p><img src="../images/tiles1.png" alt="Tiles 1 equipment" width="800" /></p>

- Take a screenshot of the device commands

<p><img src="../images/tiles2.png" alt="Tiles 2 equipment" width="800" /></p>

- Please provide the logs as text rather than a screenshot
  > [See paragraph **11**: Format correctly](https://community.jeedom.com/t/comment-nous-aider-a-vous-aider-ou-comment-poser-une-bonne-question/34932)

```
    [2020-08-24 07:37:41][DEBUG] : ┌───────── Commande trouvée pour l'équipement FREEBOX : FREEBOX - Eclairage Canapé -- Pièce : Salon (Node ID 9)
[2020-08-24 07:37:41][DEBUG] : │ Label : Enclenché -- Name : switch_state
[2020-08-24 07:37:41][DEBUG] : │ Type (eq) : light -- Action (eq): intensity_picker
[2020-08-24 07:37:41][DEBUG] : │ Index : 0 -- Value Type : bool -- Access : rw
[2020-08-24 07:37:41][DEBUG] : │ Valeur actuelle :
[2020-08-24 07:37:41][DEBUG] : │ Range : ----- -- Range color : -
[2020-08-24 07:37:41][DEBUG] : │ Name: Etat -- Type : info -- LogicalID : 0 -- Template Widget / Ligne : core::light/0-- Type de générique : LIGHT_STATE -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : │ No Repeat pour l'info avec le nom : Etat
[2020-08-24 07:37:41][DEBUG] : │ Name: On -- Type : action -- LogicalID : PB_On -- Template Widget / Ligne : core::light/1-- Type de générique : LIGHT_ON -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : │ Name: Off -- Type : action -- LogicalID : PB_Off -- Template Widget / Ligne : core::light/0-- Type de générique : LIGHT_OFF -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : └─────────
[2020-08-24 07:37:41][DEBUG] : ┌───────── Commande trouvée pour l'équipement FREEBOX : FREEBOX - Eclairage Canapé -- Pièce : Salon (Node ID 9)
[2020-08-24 07:37:41][DEBUG] : │ Label : Luminosité -- Name : luminosity
[2020-08-24 07:37:41][DEBUG] : │ Type (eq) : light -- Action (eq): intensity_picker
[2020-08-24 07:37:41][DEBUG] : │ Index : 2 -- Value Type : int -- Access : rw
[2020-08-24 07:37:41][DEBUG] : │ Valeur actuelle : 254
[2020-08-24 07:37:41][DEBUG] : │ Range : ----- -- Range color : -
[2020-08-24 07:37:41][DEBUG] : │ Name: Etat Luminosité -- Type : info -- LogicalID : 2 -- Template Widget / Ligne : /0-- Type de générique : LIGHT_COLOR -- Inverser : 0 -- Icône :  -- Min/Max : 0/255
[2020-08-24 07:37:41][DEBUG] : │ No Repeat pour l'info avec le nom : Etat Luminosité
[2020-08-24 07:37:41][DEBUG] : │ Name: Luminosité -- Type : action -- LogicalID : 2 -- Template Widget / Ligne : default/0-- Type de générique : LIGHT_SET_COLOR -- Inverser : 0 -- Icône :  -- Min/Max : 0/255
[2020-08-24 07:37:41][DEBUG] : └─────────
```
