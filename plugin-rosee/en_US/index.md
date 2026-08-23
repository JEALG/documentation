# Rosée - Givre - Trend Plug-in

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

# Description

This plugin lets you check the dew point to see if the grass will be wet in the morning, or in winter, to see if you'll need to scrape the windshield.
For this to work, you must specify a temperature sensor and a humidity sensor (outdoor ones, of course…).
It is also possible to forecast future weather trends based on past weather patterns.

# Setup

The plugin does not have any general settings; you must:

> Select a calculation method:

    - Absolute humidity
    - Freezing Point
    - Dew Point
    - Dew Point and Frost Point
    - Weather Forecast
    - Feels-like temperatures

> Fill in the required fields according to the calculation method:

    - "Temperature" Equipment (°C)
    - "Relative Humidity" (%) Equipment
    - "Wind Speed" Equipment
    - "Atmospheric Pressure" (hPa) setting: This field is required for the "Weather Trend" calculation method, and the history feature must be enabled with "Repeat identical values" set to Yes. For other calculations, the value is set to 1013.25 hPa if left blank.

<b>Optional: </b>

> - Dew Point Alert Threshold (°C): Threshold for triggering the dew point alert; default value is 2°C (dew point depression T°-Tr°). Adjust based on local observations.
> - Absolute humidity threshold: The absolute humidity threshold below which frost is unlikely to form; the default value is 2.8.
> - Temperature Offset: Adjust based on local observations and the sensor's position; default is 0.

# Frost Alert

> Sources:
>
> - <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/</a>

The plugin calculates 4 alert levels:

|  Case  | Info |
| :---: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **0** | - Calculation: None of the cases below apply<br/>- Frost Alert: 0<br/>- Dew Alert: Automatic<br/>- Digital Frost Message: 0<br/>- Info Message: No risk of frost |
| **1** | - Calculation: (Temperature <= 1 and Dew Point <= 0) and (Absolute humidity in (gr/m³) < Absolute humidity threshold)<br/>- Frost Alert: 1<br/>- Dew Alert: forced to 0<br/>- Numeric message: 1<br/>- Message: Frost unlikely despite the temperature |
| **2** | - Calculation: (Temperature <= 4 and Freezing Point <= 0.5)<br/>- Frost Alert: 1<br/>- Dew Alert: forced to 0<br/>- Digital Message: 2<br/>- Message: Risk of frost |
| **3** | - Calculation: (Temperature <= 1 and Dew Point <= 0) and (Absolute humidity in (g/m³) > Absolute humidity threshold)<br/>- Frost Alert: 1<br/>- Dew Alert: forced to 0<br/>- Numeric Message: 3<br/>- Message: Frost, Frost Detected |

# Weather Forecast

> Sources:
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

The plugin calculates 6 levels of information:

|  Level  | Trend | Widget image |
| :------: | :--------------------------------- | :----------------------------------------------------------------------: |
| <b>0</b> | Significant deterioration, unstable | <img src="../{{site.img}}/tendance_0.png" alt="Trend 0" width="40" /> |
| <b>1</b> | Deterioration, prolonged bad weather | <img src="../{{site.img}}/tendance_1.png" alt="Trend 1" width="40" /> |
| <b>2</b> | Slow decline, stable conditions    | <img src="../{{site.img}}/tendance_2.png" alt="Trend 2" width="40" /> |
| <b>3</b> | Slow improvement, stable weather   | <img src="../{{site.img}}/tendance_3.png" alt="Trend 3" width="40" /> |
| <b>4</b> | Improvement, sustainable weather   | <img src="../{{site.img}}/tendance_4.png" alt="Trend 4" width="40" /> |
| <b>5</b> | Strong recovery, unstable | <img src="../{{site.img}}/tendance_5.png" alt="Trend 5" width="40" /> |

The plugin provides two widgets for the trend:

> - Rosée/Tendance (40x40 icon) (Default widget)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Rosée/Tendance 80x80 (Icône 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>

# Feels-like temperatures

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

## More info

- **Does the plugin rely on third-party APIs?**

> No, the plugin performs the calculation internally based on temperature, humidity, and wind speed

- **Wind chill (or wind chill index)—what is it?**

> Wind chill, sometimes also called the wind factor, refers to the sensation of cold produced by the wind, even though the actual ambient air temperature does not drop.

- **What about the heat index or humidex?**

> The heat index (original English name: Heat Index (HI) or humidity) is an index developed in the United States.
>
> It combines ambient air temperature and relative humidity in shaded areas to estimate the temperature as perceived by the human body—that is, how much warmer it would feel if the relative humidity were at a different level in the shade.
>
> The result is also known as the _"air-sensed temperature"_ or _"apparent temperature"_.
>
> For example, when the temperature is 32°C (or 90°F) with 70% relative humidity:
>
> - The heat index is then 41°C (or 106°F).
> - This heat index temperature has an implied (unspecified) humidity of 20%.
> - This is the relative humidity value at which the heat index formula indicates that 41°C feels like 41 °C.
> - A heat index temperature of 32°C corresponds to an implied relative humidity of 38%.
>
> The heat index is based on the human body’s ability to cool the skin by producing sweat.
>
> This evaporates into the air, a process that requires energy, which is drawn from the environment and lowers the temperature of the boundary layer in contact with the skin, creating a cooling sensation.
>
> As relative humidity increases, evaporation becomes less efficient, resulting in a subjective sensation of increased heat. This index should not be confused with the Canadian Humidex, which uses a different formula to quantify the same effect.
