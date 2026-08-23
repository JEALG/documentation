# Tendance Baro Plugin

<img src="{{site.baseurl}}/plugin-tendance_baro/{{site.img}}/baro_icon.png" class="pluginLogo" width="100" />

## Description

This plugin calculates the upcoming weather trend based on changes in atmospheric pressure over the past few hours

## Setup

The plugin does not have any general settings.
We need to add a device to measure atmospheric pressure.

> This device must have the history feature enabled

## Weather Forecast

> Sources:
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

The plugin calculates 6 levels of information

|  Level  | Trend | Widget image |
| :------: | :--------------------------------- | :----------------------------------------------------------------: |
| <b>0</b> | Severe deterioration, unstable | <img src="../images/tendance_0.png" alt="Trend 0" width="40" /> |
| <b>1</b> | Deterioration, prolonged bad weather | <img src="../images/tendance_1.png" alt="Trend 1" width="40" /> |
| <b>2</b> | Slow decline, stable conditions    | <img src="../images/tendance_2.png" alt="Trend 2" width="40" /> |
| <b>3</b> | Slow improvement, stable weather   | <img src="../images/tendance_3.png" alt="Trend 3" width="40" /> |
| <b>4</b> | Improvement, sustainable weather   | <img src="../images/tendance_4.png" alt="Trend 4" width="40" /> |
| <b>5</b> | Strong upturn, unstable | <img src="../images/tendance_5.png" alt="Trend 5" width="40" /> |

## The plugin provides two widgets for the trend:

> - Baro/Trends (40x40 Icon) (Default Widget)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Baro/Trend 80x80 (80x80 Icon)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>
