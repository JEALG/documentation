# Temperature Plugin

<img src="{{site.baseurl}}/plugin-temperature/{{site.img}}/temperature_icon.png" class="pluginLogo" width="100" />

## Description

This plugin calculates the effect of wind on the perceived temperature (wind chill, especially when temperatures are low), as well as the discomfort caused by humidity when temperatures are high (humidex).

## Setup

The plugin does not have any general settings.
You need to add sensors for temperature, humidity, and wind speed
You can specify:

- An alert threshold for the heat index (HUMIDEX). By default, 40°C triggers the alert
- An early warning threshold for the heat index (HUMIDEX). By default, 30°C triggers the early warning.

## Feels-like temperatures

> Sources:
>
> - <a href="https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul">https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul</a>
> - <a href="http://www.meteo-mussidan.fr/hum.php">http://www.meteo-mussidan.fr/hum.php</a>

| Digital Message | Message |
| :---------------: | :----------------------------------------------------------------------------------------------------------------- |
|     <b>-7</b>     | Danger! Extremely high risk of frostbite in less than 2 minutes (see note) and hypothermia. Stay indoors |
|     <b>-6</b>     | Very high risk of frostbite within 2 to 5 minutes (see note) without full protection or physical activity |
|     <b>-5</b>     | High risk of frostbite within 5 to 10 minutes (see note) on exposed skin and hypothermia |
|     <b>-4</b>     | Moderate risk of frostbite within 10 to 30 minutes on exposed skin and of hypothermia |
|     <b>-3</b>     | Low risk of frostbite and hypothermia |
|     <b>-2</b>     | Low risk of frostbite |
|     <b>-1</b>     | No risk of frostbite or hypothermia (under normal conditions) |
|     <b>1</b> | Feeling cool or cold |
|     <b>2</b> | No discomfort |
|     <b>3</b> | A sense of well-being |
|     <b>4</b> | Varying degrees of discomfort |
|     <b>5</b> | Significant discomfort. Exercise caution. Slow down certain outdoor activities. |
|     <b>6</b> | General feeling of discomfort. Danger. Avoid exertion. |
|     <b>7</b> | Extreme danger. Work has come to a halt in many sectors. |
|     <b>8</b> | Heatstroke imminent (life-threatening). |
