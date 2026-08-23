# Plugin „Metar Infos“

<img src="{{site.baseurl}}/plugin-metar_infos/{{site.img}}/metar_infos_icon.png" class="pluginLogo" width="100" />

## Wichtig

> Diese Dokumentation wird vorübergehend hier gehostet, bis die offizielle Website wieder in Betrieb genommen wird.

## Beschreibung

Plugin zum Empfang von Wetterbeobachtungen von Flughäfen (METAR) sowie von Vorhersagen (TAF)

Ein METAR (offiziell METeorological Aerodrome Report¹ , manchmal jedoch auch als METeorological Airport Report² definiert) ist ein meteorologischer Beobachtungsbericht (keine Vorhersage) für die Luftfahrt.
Mit diesem Plugin können Sie METAR-Daten eines Flughafens abrufen und entschlüsseln. In der aktuellen Version stehen folgende Informationen zur Verfügung (die Daten hängen jedoch direkt davon ab, was vom ausgewählten Flughafen übermittelt wird):

> - Wetterlage
> - Ausführlicher Wetterbericht
> - Metadaten
> - Gültige Metar-Daten
> - UTC-Zeit des Telegramms
> - Ortszeit des Telegramms
> - Windgeschwindigkeit
> - Windrichtung
> - Windrichtung (Kurs)
> - Übersicht
> - Temperatur
> - Taupunkt
> - Luftfeuchtigkeit
> - Luftdruck
> - Wolken der Stufen 1 bis 3
> - Höhe: Wolken auf den Stufen 1 bis 3

## Konfiguration

Das Plugin erfordert keine besondere Konfiguration.

> In den Einstellungen muss der Flughafen ausgewählt oder der ICAO-Code manuell eingegeben werden

<img src="../images/choix_aeroport.png" alt="Flughafenauswahl" width="900" />

> Art der Informationen: Wählen Sie die Art der Daten aus, entweder METAR oder METAR und TAF

<img src="../images/choix_metar.png" alt="Flughafenauswahl" width="900" />
