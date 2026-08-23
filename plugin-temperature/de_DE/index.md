# Plugin „Temperatur“

<img src="{{site.baseurl}}/plugin-temperature/{{site.img}}/temperature_icon.png" class="pluginLogo" width="100" />

## Beschreibung

Dieses Plugin berechnet den Einfluss des Windes auf die gefühlte Temperatur (Windchill, vor allem bei niedrigen Temperaturen) sowie den durch die Luftfeuchtigkeit verursachten Unbehaglichkeitsfaktor bei hohen Temperaturen (Humidex).

## Konfiguration

Das Plugin verfügt über keine allgemeinen Einstellungen.
Es müssen Geräte zur Messung von Temperatur, Luftfeuchtigkeit und Windgeschwindigkeit installiert werden
Folgende Angaben sind möglich:

- Ein Alarmschwellenwert für den Hitzeindex (HUMIDEX). Standardmäßig wird der Alarm bei 40 °C ausgelöst.
- Ein Vorwarnschwellenwert für den Hitzeindex (HUMIDEX). Standardmäßig wird die Vorwarnung bei 30 °C ausgelöst.

## Gefühlte Temperaturen

> Quellen:
>
> - <a href="https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul">https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul</a>
> - <a href="http://www.meteo-mussidan.fr/hum.php">http://www.meteo-mussidan.fr/hum.php</a>

| Digitale Nachricht | Nachricht |
| :---------------: | :----------------------------------------------------------------------------------------------------------------- |
|     <b>-7</b>     | Gefahr! Extrem hohes Risiko von Erfrierungen in weniger als 2 Minuten (siehe Hinweis) und Unterkühlung. Suchen Sie Schutz |
|     <b>-6</b>     | Sehr hohes Erfrierungsrisiko innerhalb von 2 bis 5 Minuten (siehe Hinweis) ohne vollständigen Schutz und ohne körperliche Aktivität |
|     <b>-5</b>     | Hohes Risiko von Erfrierungen innerhalb von 5 bis 10 Minuten (siehe Hinweis) an ungeschützter Haut und von Unterkühlung |
|     <b>-4</b>     | Mäßiges Risiko von Erfrierungen an unbedeckter Haut innerhalb von 10 bis 30 Minuten und von Unterkühlung |
|     <b>-3</b>     | Geringes Risiko für Erfrierungen und Unterkühlung |
|     <b>-2</b>     | Geringes Erfrierungsrisiko |
|     <b>-1</b>     | Keine Gefahr von Erfrierungen oder Unterkühlung (bei normaler Exposition) |
|     <b>1</b> | Gefühl von Kühle oder Kälte |
|     <b>2</b> | Keine Unannehmlichkeiten |
|     <b>3</b> | Wohlfühlatmosphäre |
|     <b>4</b> | Mehr oder weniger starkes Unbehagen |
|     <b>5</b> | Ziemlich starkes Unbehagen. Vorsicht. Bestimmte Aktivitäten im Freien einschränken. |
|     <b>6</b> | Allgemeines Unwohlsein. Gefahr. Anstrengungen vermeiden. |
|     <b>7</b> | Äußerste Gefahr. Arbeitsniederlegung in vielen Bereichen. |
|     <b>8</b> | Drohender Hitzschlag (Lebensgefahr). |
