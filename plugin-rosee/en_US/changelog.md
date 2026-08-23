# Rosée - Givre - Trend Plug-in

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Changelog Info

### Important

> **_Please note_**: If there is no information about the update, it means that the update consists solely of documentation updates, translations, or minor bug fixes.

## 2026

### 06/03/2026

- Plugin improvement and update

## 2025

### 05/05/2025

- Added "Actual Vapor Pressure" command in Pa
_ Unit correction
- Added "mix ratio" command in g/kg: https://fr.m.wikipedia.org/wiki/Rapport_de_mélange


### 25/01/2025

- Documentation link update

### 15-16/01/2025

- Add a control unit for wind speed


### 14/01/2025

- Correction to the perceived temperature calculation: https://community.jeedom.com/t/erreur-calcul-de-la-temperature-ressentie/136577

## 2024

### 30/12/2024

- Log improvements + translation

### 28/12/2024

- Improvement log

### 01/11/2024

- Typo

### 25/09/2024

- Bug fix for setConfiguration when creating commands

### 22/09/2024

- Trend: If there is no data in the history, the trend data and numerical trend are not updated
- Translation  (Thanks @Mips)

### 14/09/2024

- Translation (Thanks, @Mips)
- PHP 8 fix

### 21/08/2024

- Translation
- Improvements and Updates to Commands
- Change to the logicalId for the frosting command (frosting => frost_point)
- Change to the logicalId for the Relative Humidity command (humidityabs => humidityabs_m3)
- Behavior: No calculation if the history is null
- CRON typo
- Log Core 4.4 Enhancements

### 28/05/2024

- Zero-value correction

### 26/05/2024

- Checking the values of specific parameters: Stop calculations if no value is present
- Improvements to logs

### 04/02/2024

- Removal of community link following Core 4.4 update
- Improvements to the display below the table

### 14/01/2024

- Improvements for Core V4.4

## 2023

### 08/10/2023

- Info Update for Community Regarding Core 4.4
- Typo

### 02/06/2023

- Market Information Update

### 02/04/2023

- Fix for Core 4.4
- The Core mini version for the plugin is 4.2

### 20230327

- Typo

## 2022

### Version 20220212

- Core Display v4.2
- Core v4.3 Feature
- The JavaScript method `jeedom.eqLogic.builSelectCmd` has been renamed correctly to `jeedom.eqLogic.buildSelectCmd`.

## 2021

### Version 20211101

- Add JSON Info
- Added pressure information and corrected command creation
- Fix for creating trend commands

### Version 20211023

- Update following the change to Core v4.2

### Version 20210728

- Improvements for Core v4.2

### Version 20210510

- Add information to the log

### Version 20210226

- Feels-like temperature correction

### Version 20210213

- Core v4.2 (beta) dashboard display
- Parent Object Correction
- General display improvements

## 2020

### Version 20201208

- Humidex Calculation Bug Fix
- Miscellaneous bug fixes

### Version 20201207

- Bug fix for command creation
- Bug Fix: Min and Max Values for Numeric Commands
- Added calculation of perceived temperature for winter https://community.jeedom.com/t/temperature-ressentie/44377/2

### Version 20201129

- Improved display, added tooltips for commands
- Improvements and Updates to Commands

### Version 20201105

- Fixed number display for thresholds and offsethttps://community.jeedom.com/t/pas-dalerte-givre/41213/8

### Version 20201031

- Improvements to the list of parent objects

### Version 20201027

- Visu Improvements on the Dashboard

### Version 20201026

- Improvements to command creation
- Improvements and Updates to Commands
- Modify command display
- Add "Reset Search" button
- Clean Log + code
- Rosee \_eqNameID Bug Fix (TEST error)
- Bug fix: removal of the "Refresh" command
- PHP Warning Correction
- Correction: Undefined variable
- Improvement if there is a history of pressure issues
- Bug fix for command creation

### Version 20200525

- Bug Fix: Recreating Commands
- Final cleanup following the relocation of documentation
- Code improvement (handling the display of parameters based on the calculation mode)

### Version 20200512

- Relocation of documentation
- Bug fix for individual registration of each device
- Registering devices after each update
- Widget modification for the trend

### Version 20200430

- Fixed: Added Core widget by default to new devices

### Version 20200418

- Added "Weather Trend" calculation
- Log cleanup
- Bug fixes
- Bug fixes related to mandatory equipment selection
- Add Cron 10/15/Hours
- Replacing Cron5 with Cron30 (calculations will be performed every 30 minutes by default)
  > **Note: Be sure to check that Cron 30 is active; if not, you'll need to enable it**
- Added Core widget for commands (for new devices only)
- Add a trend widget (only for Core V4 and newer devices)

### Version 20200409

- Separation of calculations
- Cleaning up information in the logs
- Add a button to recreate the commands
- Bug Fix: Drop-down list for calculation options is empty
- Hiding parameters is not necessary depending on the calculation mode
- Modification to command creation—this now takes the calculation mode into account
- Removal of certain intermediate calculations
- Assigning Min and Max Values to the "Digital Message"

> Note: Remember to back up each device

### Version 20200226

- The frost point is 5 if the temperature exceeds 5°
- Option to select only a portion of the calculation (Dew and frost, Absolute humidity, Frost, Dew point)
- Add a temperature offset (default value: 0)

### Version 20200210

- The dew point is equal to the temperature when the temperature is above 10°C

### Version 20200209

> _Info: Change in plugin author—thanks, @claude.metzger_

- Add additional logging in DEBUG mode
- Code cleanup
- New calculation for frost alert management
- Added a message for the frost type as well as a numeric value based on the code <A href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue</A>
  > - Case No. 0: Message = _No risk of frost_, Frost alert = _0_, Numeric message = _0_
  > - CASE 1: Message = _Frost unlikely despite the temperature_, Frost alert = _1_, Numeric message = _1_
  > - CASE No. 2: Message = _Risk of frost_, Frost alert = _1_, Numeric message = _2_
  > - CASE #3: Message = _Frost, Frost detected_, Frost alert = _1_, Numeric message = _3_
- Plugin logo update—thanks @mich0111
- Type of generic opening credits format
- Option to save the device without filling in the required fields if the device is not active
- Modify command display
  > - Added the ability to invert binary commands
  > - Deleting the message command history
- Automatically adds new commands without having to recreate them (Thanks to Kiboost and Mips)
- Change to the data type for thresholds => Numeric only
- Added an absolute humidity threshold for calculating the frost alert
- Frost information is not calculated if the temperature is above 10°C

  > _Note: You must save each device to access the new commands_


## <2020

### Version 3.3.2

- Add additional logging in DEBUG mode
- Hide visibility for dew point and frost point calculations

### Version 3.3.1

- Documentation Correction

### Version 3.3

- Bug Fix

### Version 3.2

- Added a Cron 30 (Thanks to kiboost)
- Display improvements for Core V4 (Thanks to kiboost)
- Option to rename commands (Thanks to kiboost)
- Historical Data Correction (Thanks to kiboost)
- Refresh Command (on a tile, scenario, etc.) (Thanks to kiboost)
- Improvements to logs
- Type of Generic Answer Template
- Bug Fix: Data is no longer updated if the device is disabled
- Alerts are visible by default (no longer hidden if the alert is at 0)
- Cleaning up folders (Thanks to kiboost)
- Documentation Update

> _Note: We recommend uninstalling the plugin and then reinstalling it._

### Version 3.1

- Commands are no longer retrieved for updating via `getConfiguration('data')` but rather via their `logicalId`. The commands lose their configuration data. (Thanks to jpty)

### Version 3.0

- PHP 7.3 Support
- Migration to Font Awesome 5
- Migration to Core V4 display format

### Version 2.1

- Fix for faulty dew point and frost readings

### Version 2.0

- Update for Jeedom V3 compatibility

### Version 1.5.2

- Bug fix in rosee.class.php regarding the call to the cron15() function (thanks to mika-nt28 and Mika)

### Version 1.5.1

- Bug fix related to the dew point alert threshold

### Version 1.5

- Managing dew and frost alerts based on status changes (thanks, Toregreb)

### Version 1.4

- Configurable dew point alert threshold in Information. Default value: 2°C

### Version 1.3.1

- Set the dew point and frost point alert threshold to 2°C (dew point depression)

### Version 1.3

- Added a dew point alert and a frost point alert

### Version 1.2

- Selecting temperature and humidity (via a search button) (thanks, Lunarok)

### Version 1.1

- Adding the frost sensor

### Version 1.0

- Creating the plugin
