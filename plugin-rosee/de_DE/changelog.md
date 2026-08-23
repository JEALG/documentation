# Plugin „Rosée – Givre – Trend“

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Info zum Änderungsprotokoll

### Wichtig

> **_Zur Erinnerung_**: Wenn keine Informationen zum Update vorliegen, bedeutet dies, dass es sich ausschließlich um Aktualisierungen der Dokumentation, Übersetzungen oder Korrekturen kleinerer Fehler handelt.

## 2026

### 06/03/2026

- Verbesserung und Aktualisierung des Plugins

## 2025

### 05/05/2025

- Befehl „Tatsächlicher Dampfdruck“ in Pa hinzugefügt
_ Einheitenkorrektur
- Befehl „Mischungsverhältnis“ in g/kg hinzugefügt: https://fr.m.wikipedia.org/wiki/Rapport_de_mélange


### 25/01/2025

- Link zur Dokumentation aktualisiert

### 15-16/01/2025

- Hinzufügen einer Steuerung für die Windgeschwindigkeit


### 14/01/2025

- Korrektur der Berechnung der gefühlten Temperatur: https://community.jeedom.com/t/erreur-calcul-de-la-temperature-ressentie/136577

## 2024

### 30/12/2024

- Verbesserung des Logs + Übersetzung

### 28/12/2024

- Verbesserung des Protokolls

### 01/11/2024

- Tippfehler

### 25/09/2024

- Behebung eines Fehlers bei „setConfiguration“ beim Anlegen von Befehlen

### 22/09/2024

- Trend: Wenn im Verlauf keine Daten vorhanden sind, werden die Trenddaten und der numerische Trend nicht aktualisiert
- Übersetzung  (Danke @Mips)

### 14/09/2024

- Übersetzung (Danke @Mips)
- PHP 8-Korrektur

### 21/08/2024

- Übersetzung
- Verbesserung und Aktualisierung der Steuerung
- Änderung der „logicalId“ für den Befrostungsbefehl (Befrostung => frost_point)
- Änderung der logicalId für den Befehl „Relative Luftfeuchtigkeit“ (humidityabs => humidityabs_m3)
- Trend: Keine Berechnung mehr, wenn der Verlauf null ist
- CRON-Fehler
- Verbesserung des Log-Kerns 4.4

### 28/05/2024

- Korrektur des Nullwerts

### 26/05/2024

- Überprüfung der Werte bestimmter Parameter: Abbruch der Berechnungen, wenn kein Wert vorliegt
- Verbesserung der Protokolle

### 04/02/2024

- Entfernung des Community-Links nach der Umstellung auf Core 4.4
- Verbesserung der Anzeige unter der Tabelle

### 14/01/2024

- Verbesserungen für Core V4.4

## 2023

### 08/10/2023

- Verbesserung der Informationen für die Community zu Core 4.4
- Tippfehler

### 02/06/2023

- Aktualisierung der Marktinformationen

### 02/04/2023

- Korrektur für Core 4.4
- Die Mini-Core-Version für das Plugin ist 4.2

### 20230327

- Tippfehler

## 2022

### Version 20220212

- Core-Anzeige v4.2
- Core-Funktion v4.3
- Die JavaScript-Methode „jeedom.eqLogic.builSelectCmd“ wurde korrekt umbenannt in „jeedom.eqLogic.buildSelectCmd“.

## 2021

### Version 20211101

- JSON-Info hinzufügen
- Hinzufügen von Druckangaben und Korrektur bei der Erstellung von Bestellungen
- Korrektur bei der Erstellung von Trend-Bestellungen

### Version 20211023

- Update nach der Umstellung auf Core v4.2

### Version 20210728

- Verbesserungen für Core v4.2

### Version 20210510

- Informationen zum Protokoll hinzufügen

### Version 20210226

- Korrektur der gefühlten Temperatur

### Version 20210213

- Core v4.2 (Beta) – Tabellarische Anzeige
- Korrektur des übergeordneten Objekts
- Allgemeine Verbesserung der Anzeige

## 2020

### Version 20201208

- Behebung eines Fehlers bei der Humidex-Berechnung
- Behebung verschiedener Fehler

### Version 20201207

- Behebung eines Fehlers beim Anlegen von Befehlen
- Behebung eines Fehlers bei den Min- und Max-Werten der numerischen Befehle
- Berechnung der gefühlten Temperatur für den Winter hinzugefügt https://community.jeedom.com/t/temperature-ressentie/44377/2

### Version 20201129

- Verbesserung der Anzeige, Hinzufügen von Tooltips zu den Befehlen
- Verbesserung und Aktualisierung der Steuerung

### Version 20201105

- Korrektur der Ziffernanzeige für Schwellenwerte und Offsethttps://community.jeedom.com/t/pas-dalerte-givre/41213/8

### Version 20201031

- Verbesserung der Liste der übergeordneten Objekte

### Version 20201027

- Verbesserung der visuellen Darstellung auf dem Dashboard

### Version 20201026

- Verbesserung der Auftragserstellung
- Verbesserung und Aktualisierung der Steuerung
- Anzeige der Befehle ändern
- BP-Reset zur Suche hinzugefügt
- Clean Log + Code
- Behebung des Fehlers „Rosee \_eqNameID“ (Testfehler)
- Behebung eines Fehlers beim Löschen des Befehls „Refresh“
- PHP-Warnung beheben
- Korrektur der nicht definierten Variablen
- Verbesserung bei Problemen mit dem Druckverlauf
- Behebung eines Fehlers beim Anlegen von Befehlen

### Version 20200525

- Fehlerbehebung: Neuerstellung der Befehle
- Abschluss der Bereinigung nach Verlagerung der Dokumentation
- Code-Optimierung (Anzeige der Parameter je nach Berechnungsmodus)

### Version 20200512

- Transport von Unterlagen
- Behebung eines Fehlers bei der individuellen Registrierung jedes Geräts
- Registrierung der Geräte nach jedem Update
- Anpassung des Widgets für den Trend

### Version 20200430

- Korrektur: Hinzufügen des Core-Widgets als Standard bei neuen Geräten

### Version 20200418

- Berechnung „Wettertrend“ hinzugefügt
- Reinigung des Protokolls
- Fehlerbehebungen
- Fehlerbehebungen bei der Auswahl der obligatorischen Ausrüstung
- Cron-Auftrag 10/15/Stunden hinzufügen
- Ersetzen von Cron5 durch Cron30 (die Berechnungen erfolgen standardmäßig alle 30 Minuten)
  > **Hinweis: Bitte überprüfen Sie, ob Cron 30 aktiv ist; falls nicht, müssen Sie es aktivieren**
- Hinzufügen eines Core-Widgets für die Steuerung (nur für neue Geräte)
- Widget für den Trend hinzugefügt (nur für Core V4 und neue Geräte)

### Version 20200409

- Trennung der Berechnungen
- Bereinigung der Informationen in den Protokollen
- Schaltfläche zum erneuten Erstellen der Befehle hinzugefügt
- Behebung des Fehlers: Dropdown-Liste zur Auswahl der Berechnung ist leer
- Je nach Berechnungsmodus ist das Ausblenden der Parameter nicht erforderlich
- Änderung bei der Erstellung von Bestellungen: Die Berechnungsmethode wird nun berücksichtigt
- Entfernung bestimmter Zwischenberechnungen
- Zuweisung von Minimal- und Maximalwerten für die „digitale Nachricht“

> Hinweis: Denken Sie daran, jedes Gerät zu sichern

### Version 20200226

- Der Frostpunkt beträgt 5, wenn die Temperatur über 5° liegt.
- Möglichkeit, nur einen Teil der Berechnung auszuwählen (Tau und Reif, absolute Luftfeuchtigkeit, Reif, Taupunkt)
- Temperatur-Offset hinzufügen (Standardwert: 0)

### Version 20200210

- Der Frostpunkt entspricht der Temperatur, wenn diese über 10 °C liegt

### Version 20200209

> _Info: Änderung des Autors des Plugins, danke @claude.metzger_

- Hinzufügen eines zusätzlichen Protokolls im DEBUG-Modus
- Code-Bereinigung
- Neue Berechnung für die Verwaltung der Frostwarnung
- Hinzufügen einer Meldung für die Art der Vereisung sowie eines numerischen Werts gemäß dem Code <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue</a>
  > - FALL Nr. 0: Meldung = _Keine Vereisungsgefahr_, Vereisungswarnung = _0_, Numerische Meldung = _0_
  > - FALL Nr. 1: Meldung = _Vereisung trotz der Temperatur unwahrscheinlich_, Vereisungswarnung = _1_, numerische Meldung = _1_
  > - FALL Nr. 2: Meldung = _Vereisungsgefahr_, Vereisungswarnung = _1_, numerische Meldung = _2_
  > - FALL Nr. 3: Meldung = _Reif, Reifbildung_, Reifwarnung = _1_, Numerische Meldung = _3_
- Änderung des Plugin-Logos – danke @mich0111
- Korrektur des Abspanns
- Möglichkeit, das Gerät ohne die Pflichtfelder zu speichern, wenn das Gerät nicht aktiv ist
- Anzeige der Befehle ändern
  > - Möglichkeit hinzugefügt, binäre Befehle umzukehren
  > - Löschen des Verlaufs bei Befehlen und Nachrichten
- Automatisches Hinzufügen neuer Bestellungen, ohne dass diese neu angelegt werden müssen (Vielen Dank an Kiboost und Mips)
- Änderung des Datentyps für Schwellenwerte => Nur numerisch
- Hinzufügen eines Schwellenwerts für die absolute Luftfeuchtigkeit zur Berechnung der Vereisungswarnung
- Keine Berechnung der Vereisungsdaten, wenn die Temperatur über 10 °C liegt

  > _Hinweis: Jedes Gerät muss gespeichert werden, damit die neuen Befehle verfügbar sind_


## <2020

### Version 3.3.2

- Hinzufügen eines zusätzlichen Protokolls im DEBUG-Modus
- Sichtbarkeit für die Berechnung des Taupunkts und des Vereisungspunkts ausblenden

### Version 3.3.1

- Korrektur der Dokumentation

### Version 3.3

- Fehlerbehebung

### Version 3.2

- Hinzufügen eines Cron 30 (Danke an kiboost)
- Verbesserung der Anzeige für Core V4 (Danke an kiboost)
- Möglichkeit, Befehle umzubenennen (Danke an kiboost)
- Korrektur der Verlaufsdaten (Danke an kiboost)
- Befehl „Refresh“ (auf der Kachel, im Szenario usw.) (Danke an kiboost)
- Verbesserung der Protokolle
- Standardkorrektur von Generic
- Fehlerbehebung: Die Datenaktualisierung findet nicht mehr statt, wenn das Gerät deaktiviert ist
- Warnmeldungen sind standardmäßig sichtbar (kein Ausblenden mehr, wenn der Warnwert 0 beträgt)
- Ordnerbereinigung (Vielen Dank an kiboost)
- Aktualisierung der Dokumentation

> _Hinweis: Es wird empfohlen, das Plugin zu deinstallieren und anschließend neu zu installieren._

### Version 3.1

- Die Suche nach den CMDs für das Update erfolgt nicht mehr über `getConfiguration('data')`, sondern über deren `logicalId`. Die CMDs verlieren ihre Konfigurationsdaten. (Danke an jpty)

### Version 3.0

- Unterstützung für PHP 7.3
- Umstellung auf Font Awesome 5
- Umstellung der Anzeige auf das Core-V4-Format

### Version 2.1

- Korrektur der Anzeige von Taupunkt und Fehlfunktionen der Vereisungswarnung

### Version 2.0

- Update für Kompatibilität mit Jeedom V3

### Version 1.5.2

- Behebung eines Fehlers in rosee.class.php beim Aufruf der Funktion cron15() (Vielen Dank an mika-nt28 und Mika)

### Version 1.5.1

- Behebung eines Fehlers bei der Berücksichtigung des Schwellenwerts für die Tau-Alarmstufe

### Version 1.5

- Verwaltung von Tau- und Frostwarnungen bei Statusänderungen (Danke, Toregreb)

### Version 1.4

- Der Taupunkt-Alarmschwellenwert kann unter „Informationen“ konfiguriert werden. Standardwert: 2 °C

### Version 1.3.1

- Einstellung des Alarmschwellenwerts für den Taupunkt und den Vereisungspunkt auf 2 °C (Taupunktabsenkung)

### Version 1.3

- Hinzufügen eines Taupunkt- und eines Vereisungspunkt-Alarms

### Version 1.2

- Auswahl von Temperatur und Luftfeuchtigkeit (über eine Suchfunktion möglich) (Danke, Lunarok)

### Version 1.1

- Einstellung des Frostpunkts

### Version 1.0

- Erstellung des Plugins
