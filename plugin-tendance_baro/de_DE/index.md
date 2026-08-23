# Plugin „Tendance Baro“

<img src="{{site.baseurl}}/plugin-tendance_baro/{{site.img}}/baro_icon.png" class="pluginLogo" width="100" />

## Beschreibung

Dieses Plugin ermöglicht es, die zu erwartende Wetterentwicklung auf der Grundlage der Luftdruckveränderungen der letzten Stunden zu berechnen.

## Konfiguration

Das Plugin verfügt über keine allgemeinen Einstellungen.
Es muss ein Gerät zur Messung des Luftdrucks hinzugefügt werden.

> Für dieses Gerät muss die Protokollierung aktiviert sein

## Wettertrend

> Quellen:
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

Das Plugin berechnet 6 Informationsstufen

|  Pegel  | Tendenz | Widget-Bild |
| :------: | :--------------------------------- | :----------------------------------------------------------------: |
| <b>0</b> | Starke Verschlechterung, unbeständig | <img src="../images/tendance_0.png" alt="Tendance 0" width="40" /> |
| <b>1</b> | Verschlechterung, anhaltend schlechtes Wetter | <img src="../images/tendance_1.png" alt="Trend 1" width="40" /> |
| <b>2</b> | Langsame Verschlechterung, stabiles Wetter    | <img src="../images/tendance_2.png" alt="Trend 2" width="40" /> |
| <b>3</b> | Langsame Verbesserung, stabiles Wetter   | <img src="../images/tendance_3.png" alt="Trend 3" width="40" /> |
| <b>4</b> | Verbesserung, anhaltend gutes Wetter   | <img src="../images/tendance_4.png" alt="Trend 4" width="40" /> |
| <b>5</b> | Starker Aufschwung, instabil | <img src="../images/tendance_5.png" alt="Trend 5" width="40" /> |

## Das Plugin stellt zwei Widgets für den Trend zur Verfügung:

> - Baro/Trend (40x40-Symbol) (Standard-Widget)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Baro/Tendance 80x80 (Icon 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>
