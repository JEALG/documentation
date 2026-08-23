# Plugin „Rosée – Givre – Trend“

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

# Beschreibung

Mit diesem Plugin lässt sich der Taupunkt ermitteln, um zu wissen, ob der Rasen am Morgen nass sein wird, oder im Winter, ob man die Windschutzscheibe freikratzen muss.
Damit das System funktioniert, müssen ein Gerät zur Temperaturmessung und ein Gerät zur Feuchtigkeitsmessung angegeben werden (natürlich für Außenbedingungen…).
Es ist auch möglich, die kommende Wetterentwicklung auf der Grundlage der bisherigen Wetterentwicklung zu berechnen.

# Konfiguration

Das Plugin verfügt über keine allgemeinen Einstellungen. Sie müssen:

> Wählen Sie eine Berechnungsmethode aus:

    - Absolute Luftfeuchtigkeit
    - Gefrierpunkt
    - Taupunkt
    - Taupunkt und Frostpunkt
    - Wettertrend
    - Gefühlte Temperaturen

> Füllen Sie die Pflichtfelder entsprechend der Berechnungsmethode aus:

    - Ausstattung „Temperatur“ (°C)
    - Angabe „Relative Luftfeuchtigkeit“ (%)
    - Ausstattung „Windgeschwindigkeit“
    - Einstellung „Luftdruck“ (hPa): Dieses Feld ist für die Berechnungsmethode „Wettertrend“ ein Pflichtfeld und muss die Option „Verlauf“ aktiviert haben sowie die Einstellung „Identische Werte wiederholen“ auf „Ja“ gesetzt haben. Bei anderen Berechnungen wird der Wert auf 1013,25 hPa festgelegt, sofern kein Wert eingegeben wird.

<b>Optional: </b>

> - Taupunkt-Warnschwelle (°C): Schwellenwert für die Auslösung der Taupunktwarnung, standardmäßig 2 °C (Taupunktabsenkung T°-Tr°). Je nach lokalen Beobachtungen anzupassen.
> - Absoluter Feuchtigkeitsschwellenwert: Absoluter Feuchtigkeitsschwellenwert, unterhalb dessen es unwahrscheinlich ist, dass es zu Vereisung kommt; Standardwert: 2,8.
> - Temperatur-Offset: Je nach den örtlichen Beobachtungen und der Position des Fühlers anzupassen, Standardwert 0.

# Frostwarnung

> Quellen:
>
> - <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/</a>

Das Plugin berechnet 4 Alarmstufen:

|  Fall  | Infos |
| :---: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **0** | - Berechnung: Keiner der folgenden Fälle trifft zu<br/>- Vereisungswarnung: 0<br/>- Tauwarnung: Automatisch<br/>- Digitale Vereisungsmeldung: 0<br/>- Informationsmeldung: Keine Vereisungsgefahr |
| **1** | - Berechnung: (Temperatur <= 1 und Vereisungspunkt <= 0) und (absolute Luftfeuchtigkeit in (g/m³) < Schwellenwert für absolute Luftfeuchtigkeit)<br/>- Vereisungswarnung: 1<br/>- Taupunktwarnung: fest auf 0 gesetzt<br/>- Numerische Meldung: 1<br/>- Meldung: Vereisung trotz der Temperatur unwahrscheinlich |
| **2** | - Berechnung: (Temperatur <= 4 und Vereisungspunkt <= 0,5)<br/>- Vereisungswarnung: 1<br/>- Tauwarnung: fest auf 0 gesetzt<br/>- Numerische Meldung: 2<br/>- Meldung: Vereisungsgefahr |
| **3** | - Berechnung: (Temperatur <= 1 und Taupunkt <= 0) und (absolute Luftfeuchtigkeit in (g/m³) > Schwellenwert für absolute Luftfeuchtigkeit)<br/>- Vereisungswarnung: 1<br/>- Taupunktwarnung: fest auf 0 gesetzt<br/>- Numerische Anzeige: 3<br/>- Meldung: Vereisung, Vereisung vorhanden |

# Wettertrend

> Quellen:
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

Das Plugin berechnet 6 Informationsebenen:

|  Pegel  | Tendenz | Widget-Bild |
| :------: | :--------------------------------- | :----------------------------------------------------------------------: |
| <b>0</b> | Starker Rückgang, instabil | <img src="../{{site.img}}/tendance_0.png" alt="Trend 0" width="40" /> |
| <b>1</b> | Verschlechterung, anhaltend schlechtes Wetter | <img src="../{{site.img}}/tendance_1.png" alt="Trend 1" width="40" /> |
| <b>2</b> | Langsamer Rückgang, stabiles Wetter    | <img src="../{{site.img}}/tendance_2.png" alt="Trend 2" width="40" /> |
| <b>3</b> | Langsame Verbesserung, stabiles Wetter   | <img src="../{{site.img}}/tendance_3.png" alt="Trend 3" width="40" /> |
| <b>4</b> | Verbesserung, anhaltend gutes Wetter   | <img src="../{{site.img}}/tendance_4.png" alt="Trend 4" width="40" /> |
| <b>5</b> | Deutliche Erholung, instabil | <img src="../{{site.img}}/tendance_5.png" alt="Trend 5" width="40" /> |

Das Plugin stellt zwei Widgets für den Trend zur Verfügung:

> - Rosée/Trend (40x40-Symbol) (Standard-Widget)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Rosée/Tendance 80x80 (Icône 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>

# Gefühlte Temperaturen

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

## Weitere Informationen

- **Basiert das Plugin auf APIs von Drittanbietern?**

> Nein, das Plugin führt die Berechnung intern anhand von Temperatur, Luftfeuchtigkeit und Windgeschwindigkeit durch.

- **Windchill (oder Windchill-Index) – was ist das?**

> Der Windchill-Effekt, manchmal auch als Windfaktor oder Windchill bezeichnet, beschreibt das durch den Wind hervorgerufene Kältegefühl, obwohl die tatsächliche Lufttemperatur nicht sinkt.

- **Und wie sieht es mit dem Hitzeindex oder Humidex aus?**

> Der Hitzeindex (engl. Heat Index (HI) oder „Humiture“) ist ein in den Vereinigten Staaten entwickelter Index.
>
> Es kombiniert die Raumlufttemperatur und die relative Luftfeuchtigkeit in schattigen Bereichen, um zu ermitteln, wie der menschliche Körper die Temperatur wahrnimmt, d. h. wie stark er die Wärme empfinden würde, wenn die relative Luftfeuchtigkeit im Schatten einen anderen Wert hätte.
>
> Das Ergebnis wird auch als _„gefühlte Lufttemperatur“_ oder _„scheinbare Temperatur“_ bezeichnet.
>
> Beispiel: Bei einer Temperatur von 32 °C (oder 90 °F) und einer relativen Luftfeuchtigkeit von 70 %:
>
> - Der Hitzeindex liegt dann bei 41 °C (oder 106 °F).
> - Diese Wärmeindex-Temperatur hat eine implizite (nicht angegebene) Luftfeuchtigkeit von 20 %.
> - Dies ist der Wert der relativen Luftfeuchtigkeit, bei dem laut der Wärmeindexformel eine gefühlte Temperatur von 41 °C herrscht.
> - Eine Hitzeindex-Temperatur von 32 °C entspricht einer impliziten relativen Luftfeuchtigkeit von 38 %.
>
> Der Hitzeindex basiert auf der Fähigkeit des menschlichen Körpers, die Haut durch Schweißbildung zu kühlen.
>
> Diese verdunstet in der Luft, was Energie erfordert, die der Umgebung entzogen wird und die Temperatur der an der Haut anliegende Grenzschicht senkt, wodurch ein Gefühl der Frische entsteht.
>
> Mit steigender relativer Luftfeuchtigkeit wird die Verdunstung beeinträchtigt, was zu einem subjektiven Gefühl erhöhter Wärme führt. Dieser Index darf nicht mit dem kanadischen Humidex-Faktor verwechselt werden, der denselben Effekt anhand einer anderen Formel quantifiziert.
