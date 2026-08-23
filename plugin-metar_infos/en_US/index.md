# Metar Infos Plugin

<img src="{{site.baseurl}}/plugin-metar_infos/{{site.img}}/metar_infos_icon.png" class="pluginLogo" width="100" />

## Important

> This documentation is temporarily hosted while we await the official website's return to service

## Description

Plugin that allows you to receive weather reports from airports (METAR) as well as forecasts (TAF)

A METAR (officially METeorological Aerodrome Report¹ but sometimes defined as METeorological Airport Report²) is a weather observation report (not a forecast) for aviation.
This plugin allows you to retrieve and decode METAR information from an airport. In its current version, the following information is available (though the data depends directly on what is transmitted by the selected airport):

> - Weather Report
> - Detailed weather report
> - Metar Data
> - Valid Metar
> - UTC time of the telegram
> - Telegram Local Time
> - Wind speed
> - Wind direction
> - Wind direction (bearing)
> - Visibility
> - Temperature
> - Dew point
> - Humidity
> - Atmospheric Pressure
> - Level 1 to 3 clouds
> - Altitude: Clouds, Levels 1–3

## Setup

The plugin does not require any special configuration.

> In the device settings, select the airport or manually enter the ICAO code

<img src="../images/airport_selection.png" alt="Airport Selection" width="900" />

> Information type: Select the data type—either METAR or METAR and TAF

<img src="../images/choix_metar.png" alt="Airport Selection" width="900" />
