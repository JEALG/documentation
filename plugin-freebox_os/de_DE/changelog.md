# Freebox_OS-Plugin

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />

## Info zum Änderungsprotokoll

### Wichtig

> **_Zur Erinnerung_**: Wenn keine Informationen zum Update vorliegen, bedeutet dies, dass es sich ausschließlich um Aktualisierungen der Dokumentation, Übersetzungen oder Korrekturen kleinerer Fehler handelt.
>
> **Achtung: Damit das Plugin funktioniert, muss die Freebox-Server-Version 4.8.18 installiert sein.**

### Newsfeed

> [Den Newsfeed des Plugins in der Community anzeigen](https://community.jeedom.com/t/info-plugin-Freebox-mise-a-jour-des-composants-de-la-delta-tiles-systeme/30673)

## 2026

### 27/04/2026

- Log-Verbesserung (Entfernung von Zeilenumbrüchen)

### 23/03/2026

- **Telefon**
- Befehl für Sprachnachrichten hinzugefügt

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**

### 21/03/2026

- Verbesserung des Protokolls

- **Telefon**
- Fehlerbehebung beim Anrufzähler (Rücksprung)

- **Hausautomation**
- Warnung im Bereich Hausautomation beheben, wenn das Gerät nicht vorhanden ist

### 22/02/2026

- Anrufzähler reparieren

### 01/02/2026

- Zusätzliche Informationen in den Protokollen zur Konfiguration von Schiebereglern, wenn die Maximal- und Minimalwerte nicht angegeben sind
- Korrektur der Maximal- und Minimalwerte für Schieberegler-Befehle
- Verbesserung der Protokolle für den Bereich „Titles“

### 02/01/2026

- Korrektur des USB-Anschlusses auf den VMs
- Verbesserung der Fehlermeldungen

## 2025

### 31/10/2025

- Verbesserung des Protokolls für die Festplattensuche

### 08/10/2025

- Korrektur der Ausstattungsgruppe für den Bereich Hausautomation

### 04/10/2025

- PHP-Warnung beheben

### 19/09/2025

- **WLAN**
- Hinzufügen der Liste der über WLAN verbundenen Geräte

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**


### 12/08/2025

- **Global**
- Korrektur: Cron-Eintrag, der sich bei jeder Suche nach Geräten ändert
- Migration der Mini-API auf Version 14

- **VM**
- Korrektur der VM-Abfrage (zu viele „/“ in der Abfrage)
- Behebung des Problems bei der Deaktivierung von VM-Geräten
- Korrektur der Aktion „Stopp“ – „Neustart“ – „Start“

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**
>
> **Wenn der Scan nicht durchgeführt wurde, wird möglicherweise folgende Meldung angezeigt:** Die API-Version ist nicht kompatibel ───▶︎ Fehlercode = invalid_api_version

### 15/07/2025

- Behandlung des Fehlers „Nodev“ ausschließlich im Debug-Modus (MAC-Adresse nicht gefunden)
- Verwaltung des Bridge-Modus, um bestimmte Informationen vom Player nicht abzurufen

### 12/07/2025

- **Global**
- Verbesserung der Datenwiederherstellung
- Fehlerbehebung: Standardvariable beim Aktualisieren oder Installieren des Plugins
- Behandlung von Fehlermeldungen der Freebox

- **Netzwerkverwaltung**
- Neuprogrammierung der Aktualisierung und der Gerätefunktionen Netzwerkverwaltung
- Weitere Informationen zu DHCP

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**

- **Geräteliste**
- Behebung eines Fehlers in der Liste der Netzwerkgeräte

- **LCD-Display**
- Display: Möglichkeit, die LED bei kompatiblen Boxen auszuschalten

- **Freeplugs**
- Behebung eines Fehlers bei der Datenwiederherstellung von Freeplug

- **Kindersicherung**
- Verbesserung der Kindersicherung

- **System**
- Verbesserung und Aktualisierung des Systemteils

- **WLAN**
- Verbesserung der WLAN-Statusmeldung

- **Player**
- Verbesserung des Players (sauberer Code + keine Befehle erstellen, wenn die Variable nicht vorhanden ist)

### 06/05/2025

- API-Korrektur für Player nicht verfügbar [Community-Thema](https://community.jeedom.com/t/freebox-os-messages-derreur-depuis-la-derniere-mise-a-niveau/140390?u=jag)
- Korrektur der Fehlermeldung für nicht verfügbare 4G-Module [Community-Thema](https://community.jeedom.com/t/error-message-inconnue-noent/140388?u=jag)

> **ACHTUNG: Das Plugin meldet nun keine Kommunikationsprobleme mehr zwischen Jeedom und der Freebox**
> **ACHTUNG: NEUESTE VERSION DES PLUGINS, KOMPATIBEL MIT DEBIAN 10**

### 05/05/2025

- Fehlerbehebung bei PHP <8 [Community-Thema](https://community.jeedom.com/t/call-to-undefined-function-str-contains/140353/9)

> **ACHTUNG: NEUESTE VERSION DES PLUGINS, KOMPATIBEL MIT DEBIAN 10**

### 12/08/2025

- **Global**
- Korrektur: Cron-Eintrag, der sich bei jeder Suche nach Geräten ändert
- Migration der Mini-API auf Version 14

- **VM**
- Korrektur der VM-Abfrage (zu viele „/“ in der Abfrage)
- Behebung des Problems bei der Deaktivierung von VM-Geräten
- Korrektur der Aktionen „Stopp“ – „Neustart“ – „Start“

### 04/05/2025

- **Player**
- Fügt einen Befehl zum Starten der Kanäle hinzu
- Verbesserung der Anordnung der Schaltflächen auf dem Dashboard
- Verbesserung und Aktualisierung der Steuerung
- Behebung von PHP-Warnungen und Fehlern
- Verbesserung der Auftragserstellung
- Hinzufügen des Datums, an dem der Player zuletzt im Netzwerk gesehen wurde
- Funktion „Stummschaltung“ (Ton) hinzugefügt
- Funktion zum Ändern der Lautstärke
- Zusatzinfo zur Kanalnummer
- Aktualisierung der Informationen zum Kanalnamen
- Hinzufügen der IPv4-Adresse in den Player-Einstellungen
- Hinzufügen eines Mehrfachbefehls:
      - Das Menü „Replay“ öffnen
      - Das Menü „Radio“ öffnen
      - Netflix, Prime Video, YouTube und „Meine Aufzeichnungen“ öffnen
      - Den Player mit dem zuletzt geöffneten Sender einschalten
- Möglichkeit, den Player neu zu starten

> [Vielen Dank an diese Website](https://github.com/Aymkdn/assistant-freebox-cloud/wiki/Player-API)
> [Vielen Dank an diese Ausgabe](https://github.com/JEALG/Jeedom-Freebox_OS/issues/446)
> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**
> **Neue Befehle werden nur erstellt, wenn der Player erreichbar ist**
**Der Player muss während der Suche unbedingt eingeschaltet sein und darf sich nicht im Ruhemodus (Révolution) befinden.**

- **Vernetzte Geräte**
- PHP-Warnung beheben

- **Freeplugs**
- Weitere Informationen zu den Freeplugs

- **Freigabe unter Windows und Mac**
- Zusätzliche Informationen zur Windows-Mac-Freigabe

- **Global**
- Verbesserung, Update, Anfrage zur Freebox
- Verbesserung der Rückmeldung bei Fehlermeldungen zu Anfragen

> [Vielen Dank an diese Ausgabe](https://github.com/JEALG/Jeedom-Freebox_OS/issues/446)

## 09/02/2025

- Verbesserung der Protokollierung und der Fehlermeldung für den Cron-Fehler „Hinzufügen neuer Befehle“ bei verbundenen Geräten

## 06/02/2025

- Änderung des Namens des Symbols für die Dokumentation

## 29/01/2025

- Korrektur der API-Version im Falle eines Resets: Umstellung von V10 auf v13
- Korrektur der Schaltfläche „Authentifizierung starten“
- Änderung im Plugin-Repository > [Siehe GITHUB](https://github.com/JEALG/Jeedom-Freebox_OS)
- Änderung des Plugin-Symbols

## 28/01/2025

- Migration der Mini-API auf Version 13.

### 27/01/2025

- **WLAN**
- Hinzufügen der Steuerung „Auswahl des Standby-Modus im Zeitplan“ für WLAN bei Boxen, die mit dem Eco-WLAN-Modus kompatibel sind

- **Community**
- Zusätzliche Informationen für die Community

- **Scan der Standardausstattung**
- Korrektur bei der Erstellung von Geräten vom Typ VM auf nicht kompatiblen Freebox-Geräten

> [Thema in der Community anzeigen](https://community.jeedom.com/t/api-non-compatible-avec-les-vm-sur-les-freebox-revolution/137141?u=jag)

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**

### 26/01/2025

- Aktualisierung der Links in der Dokumentation

- **WLAN**
- Hinzufügung des WLAN-Eco-Modus (für kompatible Freebox-Geräte)
- Aktualisierung der Befehlsnamen im Status der WLAN-Karten (je nach Fall muss die Suche zweimal gestartet werden)
- Korrektur des WPS-Status

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**

### 01/01/2025

- Korrekturen im Protokoll

## 2024

### 23/12/2024

- **Standardausstattung**
- Überprüfung hinzugefügt, ob eine Festplatte vorhanden ist
- Prüfung hinzugefügt, ob die Box mit den VM kompatibel ist
- Prüfung hinzugefügt, ob die Box mit den verschiedenen Anzeigetypen des Box-Bildschirms kompatibel ist

- **System**
- Festplattenstatus zu den Systemkomponenten hinzufügen

- **LCD-Display**
- Korrektur der Off-Befehlsausführung für die Ausrichtung
- Korrektur der Bildschirmhelligkeit
- Freebox Ultra Edition 25 zur Verwaltung hinzugefügt
- Korrektur des Wertes für die Textposition auf dem Display

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARDGERÄTEN DURCHGEFÜHRT WERDEN**

### 13/11/2024

- Korrektur bei der Befehlserzeugung des Players (es muss eine neue Suche gestartet werden, um den Status wieder zu erhalten)
- Korrektur bei der Einrichtung der WLAN-Steuerung

### 12/11/2024

- Verbesserung des Protokolls

- **Telefon**
- Hinzufügen von Befehlen nur für neue verpasste und empfangene Anrufe
- Behebung eines Fehlers, wenn die Liste leer ist
- Korrektur der Übersetzung

### 11/11/2024

- Korrektur bei der Erstellung der Festplatte
- Korrektur der Anfrage für das Telefon

### 10/11/2024

- Fehlerbehebung bei der Schaltfläche zum Starten der Authentifizierung
- Korrektur des Gerätetyps für Durchflussmengen
- Korrektur am Daemon: Er wird nur neu gestartet, wenn bei der Erstinstallation eine Authentifizierung stattgefunden hat.

### 27/09/2024

- Behebung eines Fehlers bei der Installation über den Market

### 25. und 26. September 2024

- Übersetzung
- Firmware im Community-Link hinzugefügt
- Sauberer Code
- PHP 8-Korrektur
- Übersetzung
- Core mini 4.2
- Behebung eines Fehlers beim Zurücksetzen der Telefonie
- Funktionsbehandlung – Veraltet
- Behebung eines Fehlers bei „setConfiguration“ beim Anlegen von Befehlen

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARD- UND ELTERNSCHUTZGERÄTEN DURCHGEFÜHRT WERDEN**

### 23/08/2024

- Behebung eines Fehlers bei der Authentifizierung

### 21/08/2024

> **ACHTUNG: ES MUSS EINE NEUE SUCHE NACH STANDARD- UND ELTERNSCHUTZGERÄTEN DURCHGEFÜHRT WERDEN**

- **Standardausstattung**

- Alle Updates wurden übernommen
- Verbesserung der Informationen für die Community zu Core 4.4
- Korrekturwarnung PHP8

- **Kindersicherung**

- Befehl für „verbundenes Gerät“ hinzufügen
- Befehl „Profilgebundene Urlaubstage“ hinzugefügt

> **ACHTUNG: Der Befehl ETAT muss gelöscht und ETAT(1) in ETAT umbenannt werden**

- **Anzeige**

- Befehle zum Erzwingen der Ausrichtung hinzugefügt
- Befehle zum Ausblenden des WLAN-Schlüssels hinzugefügt

- **System**

- Hinzufügen eines Befehls mit Informationen zum Firmware-Update des Freebox-Servers mit den folgenden Werten
      - Der Aktualisierungsvorgang wird gerade initialisiert
      - Die Firmware wird gerade aktualisiert
      - Die Firmware ist auf dem neuesten Stand
      - Beim Update ist ein Fehler aufgetreten
- Angabe der Anzeigesprache hinzufügen

- **WLAN**
- Informationen zum Eco-Modus für WLAN hinzugefügt
- Standby-Modus für die WLAN-Planung hinzugefügt

### 18/07/2024

- Verbesserung des Protokolls
- Korrektur der PHP8-Warnung

### 11/04/2024

- Behebung eines Fehlers bei der Migration von der DELTA-Box zur ULTRA-Box

### 10/04/2024

- **Allgemeines**

- Bereinigung veralteter Steuerelemente bei der Migration von Boxen (Revolution -> ULTRA, DELTA -> ULTRA).
- LOG-Verbesserung für 4.4

- **Management**

- Verbesserungsprotokoll

- **WLAN**

- Verbesserung des WLAN-Widgets zur Berücksichtigung des Energiesparmodus (Box ULTRA).

- **VM/KINDERSICHERUNG/Festplatte**

- Keine Aktualisierung des Geräts (Typ VM / Kindersicherung), wenn es auf der Freebox nicht gefunden wird, und Deaktivierung des Geräts.

- **Festplatten**

  - Keine Aktualisierung des Geräts, wenn keine Festplatte vorhanden ist, und Deaktivierung des Geräts.

- **Kacheln**

  - Falls die Box diese Funktion nicht mehr unterstützt:
      - Deaktivierung der Geräte
      - CRON GLOBAL-Titel löschen



### 15/02/2024

- Behebung eines Fehlers beim Löschen des Plugins

### 13/02/2024

- Migration der Mini-API auf Version 10.

- **Freebox Ultra nun kompatibel**
  
  - Im Bereich der Hausautomation erfolgt bei einer Umstellung von der Freebox Delta auf die Ultra keine Aktualisierung der Geräte


### 05/02/2024

- Entfernung des Community-Links nach der Umstellung auf Core 4.4
- Verbesserung der Suchleiste

### 15/01/2024

- Binäre Inversionskorrektur

### 14/01/2024

- Verbesserungen für Core V4.4

### 06/01/2024

- Verbesserung der Geräteerstellung **Netzwerkverwaltung**
- Zweiter Patch für den Bewegungssensor

### 05/01/2024

- Verbesserung des Player-Updates
- Hinzufügung des Players Mini4K/POP  **Achtung: Für diesen Player erfolgt keine Statusrückmeldung**
- Keine Aktualisierung der Geräte bei der Erstellung (beschleunigt die Erstellung)
- Tippfehlerprotokoll
- Anzeigekorrektur für Bewegungssensoren

### 03/01/2024

- Verbesserung des Player-Updates

### 01/01/2024

- Verbesserung der Informationsabruf-Funktion des Players für die Revolution

## 2023

### 17/12/2023

- Verbesserung der Informationen für die Community zu Core 4.4
- Verbesserung der Ausstattung für Core 4.4
- Wiederaufnahme, Erstellung, Bestellung, Download
- Wiederaufnahme der Systemauftragserstellung
- Korrektur der nicht definierten Variablen
- Entfernung veralteter Befehle

- **Kacheln**
  
  - Verbesserung der Wertverwaltung der Fernbedienung der Alarmanlage
  - Taste „Alarmfernbedienung“ – der Wert der Taste wird immer wiederholt
  - Verbesserung der Log-Kacheln
  - Fehlerbehebung: Aktualisierung der Info-Befehle für den Bereich TITLES
  - Verbesserung der Handhabung der Umkehrung von Binärbefehlen für den TITLES-Teil (Verwendung des Umkehrbefehls des Core)

    > **ACHTUNG: DIE SUCHE NACH TITELN MUSS ERNEUT DURCHGEFÜHRT WERDEN**

- **Vernetzte Geräte**
  
  - Behebung eines IP4-Fehlers bei deaktivierten Geräten
  - IP4 hinzufügen, wenn das Gerät eine feste IP-Adresse hat

- **Durchfluss**

  - Informationen zu Transaktionen hinzufügen (Eingehende und ausgehende)


### 04/03/2023

- Korrektur einer undefinierten Variablen
- Korrektur eines Tippfehlers im Market

### 10/02/2023

- **Allgemeines**

    > - Die API verwendet nun eine Standardvariable für alle Boxen.
    > - Änderung des nicht variablen Caches zur Verwendung des Core-Formats „pluginid::custom_key“

- **Kacheln**

    > - Behebung eines Fehlers bei der Gerätregistrierung, wenn der globale Cron-Job aktiv ist

- **Freebox Player**

    > - Behebung eines Fehlers beim Gerätestatus
    > - Hinzufügen von Informationen im Protokoll zur Unterscheidung der Player
    > - Entfernen der Aktualisierung nach dem Hinzufügen von Geräten

- **Freeplug**

    > - Korrektur des Gerätetyps

- **Gesundheit**

    > - Warnung hinzufügen, wenn DEMON NOK ist
    > - Warnmeldung anzeigen, wenn das Gerät deaktiviert ist

- **Telefon**

    > - Änderung der Funktionen „Anrufprotokoll leeren“ und „Alle als gelesen markieren“

- **Freebox-Übertragungsraten**

    > - Umstellung auf die neue API für die 4G/xDSL-Aggregation.

## 2022

### 27/11/2022

- **Allgemeines**

  > - Möglichkeit, die API-Version auf v9 zurückzusetzen, ohne den Test durchgeführt zu haben

### 24/11/2022

- **Allgemeines**

  > - Die API läuft nun standardmäßig auf allen Boxen in Version 9 (dies ist mit der Freebox Revolution kompatibel)
  > - Ergänzung des Pfads der Anfrage in der Meldung „API NICHT KOMPATIBEL: Unbekannte API-Version“

### 02/11/2022

- **Vernetzte Geräte**

  > - Fehlerbehebung im Modal-Fenster zur Port-Weiterleitung

### 29/10/2022

- **Kindersicherung**

  > - Behebung des Fehlers „API NICHT KOMPATIBEL: Unbekannte API-Version“ bei einer Aktion

### 27/10/2022

- **WLAN**

  > - Behebung eines Fehlers beim Status der WLAN-Karten
  
### 26/10/2022

- **Jeedom Mini Core-Version**

  > - Neueste mit Core 4.0 kompatible Version

- **Allgemeines**

  > - Beendigung aktiver Cron-Jobs bei refreshToken
  > - Einrichtung eines wöchentlichen Cron-Jobs zur Abfrage der gültigen API-Version
  > - Verwendung der neuesten gültigen API-Version für alle Geräte
  > - Hinzufügen einer Schaltfläche im Modal „Kopplung“, um die API-Version abzufragen
  > - Neue Funktion in Core V4.3

- **Airmedia**

  > **Für alle unten aufgeführten Neuerungen muss der Scan „Standardgeräte scannen“ gestartet werden**

    > Vollständige Überarbeitung dieses Abschnitts
    > Die alten Befehle werden entfernt, da sie nicht kompatibel sind

- **Kopplung** (21.09.2022, 22.09.2022)
  
  > - Schaltfläche zum Überspringen der Berechtigungsprüfung hinzugefügt
  > - Hinzufügen einer Schaltfläche zum Zurücksetzen der Freebox-API

- **Vernetzte Geräte** (28.08.2022)

  > - Anpassung der Reihenfolge der Geräte (zuerst die verbundenen, dann die nicht verbundenen)
  > - Überarbeitung des Befehls „refresh“ und Erstellung neuer Befehle im Hinblick auf zukünftige Verbesserungen
  > - Die folgenden Befehle werden beim nächsten Update entfernt, da sie nun in die Netzwerkverwaltung integriert sind:

    > „Feste IP-Adresse hinzufügen/löschen“
    > „Wake on LAN“

- **Netzwerkverwaltung**

  > **Für alle unten aufgeführten Neuerungen muss der Scan „Standardgeräte scannen“ gestartet werden**

  - Neue Ausstattung
  - Es vereint mehrere gemeinsame Steuerungsfunktionen, die auf verschiedene Geräte verteilt sind

  > - MAC-Filterung für WLAN verwalten
  > - „Feste IP-Adresse hinzufügen – entfernen“ für Geräte

- **Kindersicherung** (17.08.2022)
  
  > - Behebung des Fehlers bei der Suche nach neuen Steuerelementen

- **Netzwerk**

  > - Korrektur der Port-Erkennung
  > - Korrektur: MAC-Adresse zur Sperr- oder Zulassungsliste hinzufügen

- **Kacheln**

  > - Hinzufügen eines Hinweistextes zur allgemeinen Aktualisierung der Titel bei SOMFY-Rollläden
  > - Korrektur der Geräteaktualisierung, wenn der globale Cron-Job nicht aktiv ist

- **WLAN**

  > Der Befehl „Hinzufügen – Mac-Filter entfernen“ wird beim nächsten Update entfernt, da er nun in die Netzwerkverwaltung integriert ist.

### 30/04/2022

> - Änderung der Anrufliste
> - Zusätzliche Informationen zu Festplatten
> - Cron-Auftrag „Tag“ löschen
> - Möglichkeit, die Aktualisierung von Netzwerkbefehlen zu deaktivieren (davon wird abgeraten, da dies bei doppelten Befehlen zu Problemen führen kann)
> - Cron-Auftrag „Tag“ löschen

  > - Ein spezifischer Cron-Job kann bei Geräten vom Typ „Festplatte“, „vernetzte Geräte“ und „Homeadapter“ konfiguriert werden
  > - Wenn das Feld „Neue Befehle hinzufügen“ leer gelassen wird, werden keine neuen Befehle hinzugefügt

### 17/03/2022

> - Änderung bei der Erstellung einer Homeadapter-Bestellung
> - Fehlerbehebung bei der Freeplug-Gruppe
> - Einbau einer Ein-/Aus-Steuerung => Home Adapter, aber noch auf Antwort von Free warten
> - Änderung der Netzwerksuche mit Aktualisierung der Gerätenamen
> - Aktualisierung der Auftragserstellung im Netzwerk
> - Korrektur der VM-Namen bei der Erstellung

## 2021 

### 06/12/2021

> - Umbenennung des Bildordners, um den neuen Anforderungen des Core gerecht zu werden
> - Behebung eines Problems beim Löschen von Variablen im Cache
> - Verbesserung der Kameraausstattung
> - Fehlerbehebung bei den Ein- und Ausschaltbefehlen im Bereich „Titles“
> - Freeplug hinzufügen,

  > - Info: Funktion des Freeplug
  > - Aktion „Zurücksetzen“
  >   **Für alle unten aufgeführten Neuerungen muss ein Scan der Standardgeräte durchgeführt werden**
  >   Um die Freeplugs nutzen zu können, müssen sie unbedingt gekoppelt sein

### 04/08/2021

- Behebung eines Fehlers beim Aktualisieren des Alarms

### 29/07/2021

- Behebung eines Fehlers bei den Befehlen für virtuelle Maschinen
- Korrektur Airmedia
- Verbesserungen für Core 4.2

### 27/06/2021

- **Freebox-Übertragungsraten**

  > - Behebung des Problems bei der Aktualisierung der Glasfaserdaten auf den Freebox Revolution-Geräten

- **Downloads**

  > - Behebung eines Problems bei den Modus-Steuerelementen des Downloads
    > **Die alten Befehle werden beim Update gelöscht. Sie müssen den Standard-Gerätescan ausführen, um den neuen Befehl zu erhalten.**

### 28/05/2021

- Behebung des Problems, dass Cron bei einer Aktualisierung des Tokens angehalten und nicht neu gestartet wurde
- Änderung des Wertes des Befehls „Fehler“ des Alarms, wenn dessen Wert null ist
- Verbesserung der Suche nach vernetzten Geräten

### 23/05/2021

- Korrektur der Funktionsweise der Slider-Umkehrung
- Korrektur der Ein- und Ausschaltbefehle für alle WLAN-Befehle
- Korrektur der Vorlage für die mobile Version des Netzwerks
- Verbesserung der WLAN-WPS-Steuerung

### 10/05/2021

- Korrektur: Kindersicherung
- Verbesserung der Aktionskacheln (Typ „bool“)

### 08/05/2021

- Korrektur, Zurücksetzen, Kopplung

### 07/05/2021

- Verbesserung der Geräteerstellung (Behandlung von Duplikaten)
- Verbesserung der Ausrüstungsliste
- Behebung von Fehlern bei der Erstellung von Systemgeräten auf der Freebox Revolution
- Bridge-Modus: Die folgenden Geräte werden nicht angelegt

  > - Air Média
  > - Vernetzte Geräte
  > - Geräte mit WLAN-Zugang für Gäste
  > - Downloads
  > - WLAN

- **Verbesserung von Cron/DEMON**

  - Dämon-Verbesserung
  - Cron-Eintrag für Aktionen hinzugefügt, um die Langsamkeit der Freebox auszugleichen (Danke an @Nebz und @Foulek57)
  - Verbesserung des Cron-Refresh-Tokens

- **Verbesserungen durch die Freebox-Firmware 4.3**

- **Kindersicherung**

  > - Aktualisierung der Berechtigungsprüfung beim Pairing

- **System**

 > - Hinzufügen von Sprachinformationen zur Freebox

- **Vernetzte Geräte**

  > - Berücksichtigung neuer Gerätetypen (vernetzte Fahrzeuge)

- **VM**

  > - Gerät hinzufügen (Status, Start, Stopp, Neustart und weitere Informationen)

- **Windows/Mac-Freigabe**

  > - Möglichkeit, SMBv2 zu aktivieren
      > Wenn SMBv2 aktiviert ist, werden die Befehle zur Druckerfreigabe bei der nächsten Aktualisierung des Geräts gelöscht.
      >
      > Achtung: Wenn Sie diese Funktion aktivieren, funktionieren die Jeedom-Backups möglicherweise nicht mehr, wenn Sie auf der Freebox sichern.

- **Kacheln**

  > - Hinzufügen eines globalen Cron-Refreshs für den Bereich Hausautomation (danke an @Nebz und @Foulek57)
  > - Behebung eines Fehlers beim Anlegen von Kameras
    > **Achtung: Es kann vorkommen, dass Kameras im Camera-Plugin doppelt angelegt werden.**
  > - Behebung eines Fehlers beim Anlegen von Steckdosen
  > - Symbol für Geräte hinzugefügt (danke @Skillix)
  > - Verbesserung der Steuerung verschiedener Rollladentypen

  > - Toggle-Funktion für bestimmte Rollladentypen hinzugefügt
  > - Behebung eines Fehlers bei der Umkehrung der numerischen Befehle
  > [Den Newsfeed des Plugins in der Community anzeigen](https://community.jeedom.com/t/info-plugin-Freebox-mise-a-jour-des-composants-de-la-delta-tiles-systeme/30673/54?u=jag)

> **Für alle oben genannten Neuerungen müssen alle Scans gestartet werden**

### 16/02/2021

- Debug-Menü für Boxen hinzugefügt, die Tiles unterstützen (Freebox Delta)

### 14/02/2021

- Core v4.2 (Beta) – Tabellarische Anzeige
- Korrektur der Suche nach Kindersicherung

- **Serienausstattung**

  > - Hinzufügen des Geräts „LCD-Display“ ausschließlich für Freebox Revolutions
    > **Für alle unten aufgeführten Neuerungen muss ein Scan der Standardgeräte durchgeführt werden**

- **Kacheln**

  - **Homeadapter**

    - Verbesserung der Aktualisierung von Bestellungen
    - Behebung eines Fehlers beim Anlegen von Aufträgen

  - **Seite „Gesundheit“**
    - Verbesserung der Anzeige
    - Behebung eines Fehlers bei der Anzeige des Akkustands der Fernbedienungen für die Alarmanlage

### 23/01/2021

- **Kacheln**

  > **Für alle unten aufgeführten Neuerungen muss ein „Scan Tiles“ gestartet werden**

  - **Alarm**

    - Fehlerbehebung: Statusmeldungen für Homebridge wurden nicht aktualisiert

### 22/01/2021

- Verbesserung der Suche nach zusätzlichen Steuerungen für Geräte
- Verbesserung der Darstellung des Authentifizierungsbereichs auf Mobilgeräten

- **Vernetzte Geräte**

  - Hinzufügen des Befehls zum Zuweisen einer **_festen IP-Adresse_** aus einem Szenario heraus
    > Man muss eine **Suche nach Zusatzgeräten** durchführen, um die neuen Befehle zu erhalten

- **Kacheln**

  > **Für alle unten aufgeführten Neuerungen muss ein „Scan Tiles“ gestartet werden**

  - **Kamera**

    - Hinzufügen dieses Geräts zum Plugin mit folgenden Möglichkeiten:
      - Aktivieren / Deaktivieren:

        > - Bewegungserkennung
        > - Zusammen mit dem Alarm aktivieren
        > - HD-Qualität
        > - Vertikal drehen
        > - Zeitstempel
        > - Geräuscherkennung
        > - RTSP-Stream

      - Einstellungen:

        > - Empfindlichkeit
        > - Schwellenwert
        > - Empfindlichkeit des Mikrofons
        > - Lautstärke des Mikrofons

    - Die Kamera wird automatisch zum Kamera-Plugin hinzugefügt, sofern dieses vorhanden ist

      > - Behebung eines Fehlers beim Erstellen der Kamera im CAMERA-Plugin

  - **Fernbedienung**

    - Hinzufügen des Batterietyps zur Ausrüstung
    - Funktion hinzugefügt: Gerät aktiviert

  - **Bewegungs- und Öffnungsmelder**

    - Folgende Funktionen wurden hinzugefügt:
      - Aktivieren / Deaktivieren für:

        > - Zeitgesteuerter Bereich
        > - Hauptalarm
        > - Zweiter Alarm

    - Umkehrung des Zustands der Bewegungsmelder, um die Kompatibilität mit Homebridge zu gewährleisten
    - Hinzufügen des Batterietyps zur Ausrüstung

  - **Alarm**

    - Folgende Funktionen wurden hinzugefügt:
      - Einstellungen:

        > - Lautstärke der Signaltöne
        > - Leistung der Sirene
        > - Verzögerung vor der Aktivierung
        > - Verzögerungszeit mit Sirene
        > - Dauer des Sirenensignals

    - Verbesserung der nicht funktionierenden Alarmfunktion mit Homebridge

      > - **Um die Verbesserungen zu erhalten, muss die Ausrüstung des Alarmsystems gesichert werden**
      > - **Ohne diese Sicherung funktioniert das Homebridge-System nicht mehr**

    - Hinzufügen des Batterietyps zur Ausrüstung

## 2020

### 13/12/2020

- Fehlerbehebung bei der Suche nach Durchflussmessgeräten

### 09/12/2020

- Behebung eines Fehlers, durch den der Alarm mit Homebridge nicht funktionierte
  > Um dieses Problem zu beheben, muss eine erneute Suche nach den Tiles gestartet werden

### 08/12/2020

- **Vernetzte Geräte**

  - Hinzufügen des Befehls zum Starten einer **_Suche nach neuen Geräten_** aus einem Szenario heraus
  - Hinzufügen des Befehls zum Starten von **_Wake on LAN_**; diese Funktion ist über ein Szenario verfügbar (auf Anfrage von @mguyard)

    > Man muss eine **Suche nach Zusatzgeräten** durchführen, um die neuen Befehle zu erhalten

- **WLAN**

  - Korrektur der WLAN-Statusrückmeldung
  - Status der verschiedenen WLAN-Karten hinzufügen

- **Allgemeines**

  - Korrektur der Suchschaltfläche für Systemgeräte

### 29/11/2020

- **WLAN**

  - Unterstützung für die Verwaltung der MAC-Filterung hinzugefügt
  - Möglichkeit, MAC-Adressen in der MAC-Filterverwaltung über ein Szenario hinzuzufügen oder zu entfernen
  - Hinzufügen einer MAC-Adressfilterung: Whitelists / Blacklists (diese Filterung erfolgt pro Szenario)

  > Man muss eine **Suche nach Zusatzgeräten** durchführen, um die neuen Befehle zu erhalten

- **Vernetzte Geräte**

  - Hinzufügen des Befehls zum Starten einer **_Suche nach neuen Geräten_** aus einem Szenario heraus
  - Hinzufügen des Befehls zum Starten von **_Wake on LAN_**; diese Funktion ist über ein Szenario verfügbar (auf Anfrage von @mguyard)

    > Man muss eine **Suche nach Zusatzgeräten** durchführen, um die neuen Befehle zu erhalten

- **Allgemeines**

  - Optimierung der Geräteerstellung
  - Allgemeine Verbesserung der Anzeige gemäß der Jeedom-Vorlage
  - Hinzufügen von Tooltips zu den Befehlen

### 06/11/2020

- Verbesserung der Liste der übergeordneten Objekte
- Hinzufügen der Seite „Zustand“ für Geräte
  > Bitte beachten Sie, dass der Akku bei bestimmten Geräten (Fernbedienung, Bewegungsmelder) nicht unterstützt wird.

### 28/10/2020

- Korrektur der Aktualisierung des 4G-Status
- Verbesserung der Kacheln

### 15/10/2020

> **Vielen Dank**
> Vielen Dank an die Beta-Tester: ipapy, Tom's, Olive, Jcamus86 und Noodom für ihre Unterstützung und ihr Feedback

- **Festplatte**

  - Überarbeitung dieses Abschnitts, um Festplatten mit Partitionen zu unterstützen

- **WLAN**

  - Hinzufügen einer WPS-WLAN-Steuerung
    > Man muss eine **Suche nach Zusatzgeräten** durchführen, um die neuen Befehle zu erhalten

- **Kacheln**

  - Behebung eines Fehlers beim Anlegen von Aufträgen

- **Optimierung**

  - Berücksichtigung der Geräteversionen bei der Aktualisierung des Plugins
  - Verbesserung des Protokolls „Sitzung schließen“

### 14/10/2020

> **Vielen Dank**
> Vielen Dank an die Beta-Tester: ipapy, Tom's, Olive, Jcamus86 und Freetronic für ihre Hilfe und ihr Feedback
>
> Vielen Dank an Mips für seine Hilfe bei der Optimierung des Codes, um Fehlermeldungen zu vermeiden

- **Festplatte**

  - Berücksichtigung der Verbesserungen von @mid.sebastien

  > **Achtung: Die Konfiguration jedes Geräts muss geändert werden**

<p><img src="../images/changelog_disque.png" alt="Festplatte" width="450" /></p>

- **Optimierung**

  - Freebox Débit: Optimierung der Anzahl der Anfragen
  - Verbesserung des Refresh-Tokens zur Anpassung an die neue Firmware der Freebox
  - Korrekturen bei undefinierten Variablen im Bereich „Tiles“
  - Korrekturen bei Nullwerten
  - Cron
    - Cron-Aufträge werden nicht ausgeführt, wenn das Gerät deaktiviert ist
    - Hinzufügen eines zusätzlichen Protokolls bei Problemen mit einem Cron-Job

### 01/10/2020

> **Vielen Dank**
> Vielen Dank an die Beta-Tester: ipapy, Tom's, Olive und Jcamus86 für ihre Unterstützung und ihr Feedback
>
> Vielen Dank an Mips für seine Hilfe bei der Optimierung des Codes, um Fehlermeldungen zu vermeiden

- **System**

  - Folgende Informationen hinzufügen
    - Name: Freebox
    - Feeebox-Modus
    - IP
  - Optimierung der Datenabfrage (weniger Abfragen)

- **Vernetzte Geräte**

  - Diese Funktionen sind nur verfügbar, wenn sich die Freebox nicht im Bridge-Modus befindet.
    > Wenn Sie sich im Bridge-Modus befinden, müssen Sie die beiden Geräte manuell aus der Liste der verbundenen Geräte löschen (Gast-WLAN und LAN).
  - Optimierung der Aktualisierung und der Erstellung von Bestellungen
  - Cron Daily: Neu erkannte Geräte sind unsichtbar

- **Cron**

  - Der Cron-Job wird nicht ausgeführt, wenn der Daemon _nok_ ist.
  - Optimierung des Cron-Jobs

- **CronDaily**

  - Der Cron-Job wird nicht ausgeführt, wenn der Daemon _nok_ ist.
  - Cron sucht nicht nach verbundenen Geräten, wenn sich die Freebox im Bridge-Modus befindet
    > Vergessen Sie nicht, einen Scan der Standardgeräte durchzuführen

- **Kopplung**

  - Hinzufügen eines Links in jedem Fenster zur Dokumentation des Plugins
  - Hinzufügen eines Links zur Freebox-Benutzeroberfläche, falls die Berechtigungen nicht stimmen

- **PHP-Optimierung**

  - Behebung von Fehlern in den Protokollen im Info-Modus
  - Behebung von Divisionen durch Null

### 12/09/2020

- Möglichkeit, die Zahlenwerte umzukehren (Aktion und Info)
- Widget „Festplatte und Netzwerk“ zwangsweise entfernen
- Entfernung der 4G-Datenmengen (Die Daten werden nicht an die API übermittelt)
- Behebung des Authentifizierungsproblems nach der neuen Firmware-Version 4.2.5 für die Freebox-Server

- **Freebox-Übertragungsraten**

  - Optimierung der Datenwiederherstellung

- **Player**

  > Nach dem Update müssen die Geräte entfernt werden.

  > **Status (ein oder aus)**:
  >
  > - Der Befehl wird nur erstellt, wenn der Player seinen Status zurückgibt.
  > - Der Player muss unbedingt eingeschaltet sein und darf sich nicht im Ruhemodus befinden. (Révolution)
  > - Der Player mini4K ist nicht kompatibel, der Player POP ist noch nicht kompatibel

### 30/08/2020

- Fehlerbehebungen: Generischer Fehler bei den WLAN-Planungsbefehlen
- Fehlerbehebung bei der Suche nach WLAN-Geräten im Gastmodus
- Korrekturen bei der Bedienung der Tiles
- Korrekturen: Farbslider inaktiv
  > Der Befehl „Farbschieberegler“ muss entfernt und eine Suche nach den Kacheln durchgeführt werden, um diese Korrektur vorzunehmen.

### 29/08/2020

- **Freebox-Übertragungsraten**

  - Wiederaufnahme der Befehle aufgrund von Unterschieden zwischen den Boxen und den Protokollen
    > Die Befehle werden beim Scan der Standardgeräte aktualisiert.
  - Hinzufügen der ADSL-Daten

- **System**

  - Hinzufügen des Namens der Schaltfläche auf dem Dashboard für den Befehl „Reboot“

- **Kopplung**

  - Zusätzliche Informationen, wenn die Verknüpfung neuer Anwendungen deaktiviert ist
  - Anpassung des Fortschrittsbalkens während des Pairings
  - Protokoll hinzufügen
  - Hinzufügen einer Meldung, falls in Ihrem Jeedom kein Name vorhanden ist

- **Downloads**

  - Hinzufügen der Information zum Verbindungsstatus
  - Hinzufügen der Info zum Planungsstatus
  - Hinzufügen der Statusinformation zum Download-Modus
  - Befehle zum Ändern des Betriebsmodus (4 Modi) hinzugefügt

- **Player**

  - Einige Player geben ihren Namen nicht zurück. Einrichtung einer Ausweichlösung, um das Equipment erstellen zu können
    > Die Befehle werden beim Scan der Standardgeräte aktualisiert.
  - Eintrag in den Protokollen hinzufügen, wenn die Player-ID leer ist

  ```
  Player : Freebox-Mini-52ec41c5c8d0bbee -- L'Id est vide donc pas de création de l'équipement (mettre sous tension le Player pour résoudre ce problème)
  ```

- **Kacheln**

  - Möglichkeit, die Steuerung für Schieberegler-Aktionen umzukehren
    > Damit dies funktioniert, müssen der Mindest- und der Höchstwert angegeben werden.

### 26/08/2020

- Behebung eines Fehlers, der beim Update zu einer Endlosschleife führte
- Behebung eines Fehlers bei der Datenübertragungsrate: 4G-Datenübertragungsraten werden nicht mehr hinzugefügt, wenn die Karte nicht vorhanden ist
- Korrektur der Reihenfolge der Abbuchungsaufträge

### 25/08/2020

> **Wichtig**
> **Die Freebox muss im neuen Menü erneut gekoppelt werden**
>
> **FÜHREN SIE DAS UPDATE NICHT DURCH, WENN SIE NICHT ZU HAUSE SIND**

> **Vielen Dank**
> Vielen Dank an die Betatester: ipapy, Tom's, Olive und jcamus86 für ihre Hilfe und ihr Feedback
>
> Danke, Titi_Titi, dass du mir hilfst, das Plugin zu verbessern

- Verbesserung der Fehlermeldungen (im Fehlerfall wird eine Meldung im Meldungscenter angezeigt)
- Entfernen nicht mehr verwendeter Widgets
- Behebung von Fehlern beim Befehl „Aktualisieren“ bei bestimmten Geräten
- Funktionen, die für die Box nicht verfügbar sind, werden ausgeblendet (z. B.: Tiles scannen)
- Leere Gerätegruppen werden ausgeblendet
- **Täglicher Cron-Job**
  - Täglicher Cron-Job hinzugefügt, um nach neu verbundenen Geräten zu suchen
  - Täglicher Cron-Job zum Suchen nach neuen Datenträgern hinzugefügt
  - Täglicher Cron-Job hinzugefügt, um nach neuen Home Adaptern zu suchen
- **Kopplung**
  - Einrichtung eines modalen Fensters zur Erleichterung der Kopplung (Verbindung) mit der Freebox
    > Das Menü befindet sich nun in der Benutzeroberfläche des Plugins
    > Die Dokumentation des Plugins wurde entsprechend aktualisiert [Siehe Dokumentation](https://mika-nt28.github.io/Documentations/freebox_OS/fr_FR/?theme=light#tocAnchor-1-2-1)
  - Änderung der Standardeinstellungen (Ausblenden nicht benötigter Parameter)
  - Hinzufügen einer Funktion zur Überprüfung der Berechtigungen; bei **NOK** ist es nicht möglich, fortzufahren (erforderliche Berechtigungen sind fett gedruckt)
  - Für die Freebox Delta: Es ist möglich, die Räume der Freebox mit den Objekten von Jeedom zu verknüpfen
  - Möglichkeit, nach Abschluss der Authentifizierung die Suche nach den verschiedenen Geräten zu starten
- **Telefon**
  - Entfernung aller veralteten Befehle
    > Die Befehle werden beim Aktualisieren des Plugins gelöscht.
  - Widgets entfernen
  - Behebung des Problems mit den Zeilenumbrüchen bei der Anzeige von Anruflisten
- **Freebox-Übertragungsraten**
  - Umbenennung von Befehlen
    > Die Befehle werden beim Scan der Standardgeräte aktualisiert.
  - Hinzufügung von „Ping-Antwort-Info“ und „Proxy Wake on LAN“
  - Hinzufügen spezifischer Befehle für Glasfaser (wird nur hinzugefügt, wenn das Modul _ftth_ vorhanden ist)
  - Hinzufügen spezifischer Befehle für Verbindungen vom Typ _xDSL + 4G_
- **Vernetzte Geräte**
  - Lösung für das Problem, dass Geräte, die nicht in der Freebox vorhanden sind, nicht gelöscht werden
  - Cron-Auftrag „Tag“ hinzugefügt, um nach neuen Geräten zu suchen.
  - Möglichkeit, IP-Adressen im Widget zu verbergen
  - Das Widget wurde umbenannt
    > Man muss nach **zusätzlichen Geräten** suchen, um das neue Widget zu erhalten.
- **Downloads**
  - RSS-Feed hinzufügen
- **Festplatte**
  - Das aktuelle Widget entfernen und das Standard-Core-Widget verwenden
- **WLAN**
  - Entfernung der Schaltfläche „WLAN aktivieren/deaktivieren“
    > Zur Verwaltung des WLANs müssen die Befehle „ON“ und „OFF“ verwendet werden
- **Kamera**
  - Verbesserung der Kameraeinstellungen
    > Das Gerät muss entfernt werden, um die neuen Einstellungen zu erhalten.
  - Unterdrückung der Installationsmeldung der Kamera, wenn diese erkannt wird
- **Kacheln**
  - Behebung eines Problems bei der Suche
- **Serienausstattung**
  - Behebung eines Problems bei der Suche
- **Freebox-Übertragungsraten**
  - Hinzufügen von Informationen zu IPv4 und IPv6
    > Man muss noch einmal nach den Standardgeräten suchen, um diese Information zu erhalten.
- **Ausstattung – WLAN-fähige Geräte – Gast**
  - Diese Ausrüstung hinzufügen

### 06/08/2020

> Nach dem Update der Freebox auf Version 4.2.3

- IP-Korrektur für Freebox

### 29/07/2020

> **Vielen Dank**
> Vielen Dank an die Beta-Tester: ipapy, Tom's, Olive und jcamus86 für ihre Hilfe und ihr Feedback
>
> Danke, Titi_Titi, dass du mir hilfst, das Plugin zu verbessern

> **Damit das Plugin funktioniert, muss die Freebox-Server-Version 4.2 installiert sein**

- Überarbeitung des Abschnitts zur Erstellung von Standardgeräten
- **Kindersicherung**
  - Möglichkeit, für einen ausgewählten Zeitraum zu sperren oder zu entsperren
    > Um diese neuen Funktionen nutzen zu können, müssen Sie die Geräte unter „Kindersicherung“ entfernen und eine neue Suche durchführen.
- **Alle Kacheln**
  - Korrektur der Steuerung von Rollläden vom Typ „Slider“
- **Download**
  - Korrektur der Download-Zahl, der Wert war immer leer
- **Festplatte**
  - Verbesserung der Namensgebung bei der Erstellung des Geräts
  - Behebung des Problems, dass die Festplattenkapazität nicht zurückgesetzt wurde
- **Gesamte Ausstattung**
  - Zuweisung unterschiedlicher Aktualisierungszeiten (Cron) je nach Gerätetyp.
    > Dies gilt ausschließlich für neue Geräte

### 24/07/2020

> **Achtung: Damit das Plugin funktioniert, muss die Freebox-Server-Version 4.2 installiert sein.**
>
> **Außerdem müssen die Berechtigungen in der Freebox-Konsole aktualisiert werden**
>
> Achtung: Der Befehl „WLAN aktivieren/deaktivieren“ wird bei den nächsten Updates entfernt. Zur Verwaltung des WLANs müssen Sie künftig die Befehle „ON“ und „OFF“ verwenden.

> **Vielen Dank**
> Vielen Dank an die Betatester: ipapy, Tom's, Olive und jcamus86 für ihre Hilfe und ihr Feedback
>
> Danke, Titi_Titi, dass du mir hilfst, das Plugin zu verbessern

- Reinigung, Erstellung von Aufträgen
- Symbol für Akkus hinzugefügt
- Migration aller APIs auf V8
- Überarbeitung der Abschnitte „Update“ und „Refresh“
- Erstellung einer Template-Klasse sowie Refresh und Update
- Reinigung der APIs
- Erstellung der Klasse „Freebox_OS.inc“
- Behebung eines Fehlers beim Anlegen von Bestellungen für Datenträger
- **Umbenennung von Geräten**
  - _ADSL_ wird zu _Freebox Débits_
  - _AirPlay_ wird zu _Air Media_
  - _Netzwerk_ wird zu _vernetzte Geräte_
- **Alarm**
  - Behebung eines Fehlers im Freebox-Alarm-Widget
  - Hinzufügen von Namen und Symbolen für die Modi
  - Erstellung spezifischer Befehle zur Integration in Homebridge

    > - Es wird dringend empfohlen, dieses Gerät zu entfernen, um die neuen Befehle zu erhalten.

- **Fernbedienung für die Alarmanlage**
  - Abruf des letzten Status
- **System**
  - Übermittlung der neuen Statusmeldungen
    > Es wird empfohlen, das Gerät zu entfernen und nach Standardgeräten zu suchen.
- **4G**
  - Befehl zum Aktivieren/Deaktivieren von 4G auf der Box hinzugefügt
    > Befehle werden nur hinzugefügt, wenn die Karte erkannt wird
- **WLAN**
  - Planung hinzufügen => Status + Aktivieren + Deaktivieren
  - Hinzufügen eines Generiktyps für WLAN (um es über Homebridge zu steuern)
- **Kindersicherung**
  - Hinzufügen der Kindersicherung => Status
  - Hinzufügen der Befehle „Entsperren“ / „Sperren“ (30 Min./1 Std./2 Std.)
- **Kamera**
  - Aktualisierung der Hersteller- und Modellangaben nach der Integration in das Kamera-Plugin
- **Vernetzte Geräte**
  - Widget unterstützt neue Gerätebilder
  - Behebung von Fehlern bei der Verwaltung leerer Ports
- **Alle Kacheln**
  - Fehlerbehebungen bei den Schiebereglern für die Beleuchtung
    > Man muss die Befehle unbedingt löschen, um dieses Problem zu beheben.

### 05/07/2020

- Behebung eines Fehlers bei der Transparenz von Netzwerkgeräten und Festplatten
- Behebung eines Fehlers im Status der HomeAdapter
- Kompatibilität mit V3 für bestimmte Symbole
- Ausrichtung der Symbole für die Alarmsteuerung entsprechend dem Alarm-Plugin
- **Kamera**
  - Protokollierung bei der Erstellung
  - Änderung der Kameraeinstellungen beim Anlegen des Geräts im **_Kamera-Plugin_** – dies ermöglicht eine bessere Integration in Homebridge.
    > Bitte beachten Sie, dass die Einstellung an der vorhandenen Anlage nicht geändert wird.
    >
    > - Entweder muss das Gerät entfernt und ein erneuter Scan der Tiles gestartet werden
    > - Ändern Sie entweder die folgenden Einstellungen:
    >   - **URL des Streams**: rtsp://#Benutzername#:#Passwort#@#IP-Adresse#/img/live
    >   - **Bildfrequenz des Videos** _(Registerkarte „Aufnahme“)_: 15

### 02/07/2020

- **WLAN**
  - Weiterleitung von Befehlen an ein bestimmtes WLAN-Gerät
    > Achtung: Dieses Gerät ist standardmäßig deaktiviert.
  - Symbol für die Ein- und Ausschaltfunktionen hinzugefügt
  - Widget für den Status und die Ein-/Aus-Funktion des WLANs hinzugefügt (nur für V4)
  - Umstellung der API von V3 auf V5
- **Telefon**
  - Verbesserung des Widgets
  - Hinzufügen von Symbolen für die verschiedenen Befehle (in Farbe für V4)
- **Download**
  - Hinzufügen von Symbolen für die verschiedenen Befehle (in Farbe für V4)
  - Zuordnung der Core-Widgets zu den verschiedenen Befehlen
- **Systeme**
  - Symbole für Temperaturen und Lüfter hinzugefügt
  - Hinzufügen von Symbolen für die Schaltflächen „Update“ und „Neustart“ (in Farbe für V4)
  - Korrekturen am Subtyp der Geräte
  - Aktualisierung der Minimal- und Maximalwerte bestimmter Befehle
- **Airplay**
  - Hinzufügen von Stopp- und Wiedergabe-Symbolen (nur für Neuinstallationen, in Farbe für V4)
- **Kacheln**
  - Helligkeitsfehler 0 bis 255 + Anzeige von Min./Max.-Werten auf den digitalen Bedienelementen
  - Hinzufügen eines BP vom Typ „Switch/Toggle“
  - Verknüpfung von Aktionen und Befehlen für die Typen „Jalousien“ und „Beleuchtung“
  - Verschiebung der Suchfunktion „Homeadapter“ in die Tiles-Suche (nur für Freebox DELTA erforderlich)
  - Zusammenführung der Funktionen „Tiles“ und „Homeadapter“
  - Verbesserung des Widgets für den Alarm
  - Hinzufügen von Informationen zum Aktionstyp und zum Gerät
    > Man muss auf „Scan Tiles“ klicken, um diese Informationen zu erhalten.
- **Korrekturen und Verbesserungen**
  - Fehlerbehebung: **Zahnrad dreht sich endlos bei Aktivierung des Plugins**
  - Deaktivierung der Geräteerstellung bei der Erstinstallation
  - Befehl zum Suchen der Freebox-Systemgeräte hinzugefügt
  - Hinzufügen einer Netzwerkanalyse nach der Suche nach Systemgeräten
  - Ergänzung in der Befehlsliste: Symbol, Min.-Max.
  - Deaktivierung der Geräteerstellung bei der Erstinstallation
    > Klicken Sie auf „Standardgeräte scannen“.

### 11/06/2020

- Fehlerbehebung: Anzeige des Akkustands: Standardmäßig ausgeblendet
- Fehler: Standardvorlage für Sabotage und Öffnen
- Fehler: Umkehrung des Standardwerts auf dem Deckel + Zuweisung der Vorlage
- Fehler: Präsenzmelder – Korrektur der Vorlagen und Umkehrung der Signale
- Berechtigung zum Löschen von Bestellungen

### 09/06/2020

- Änderung der Batteriealarmmeldung bei der Erstellung des Auftrags

### 07.06. und 08.06.2020

- Geräte vom Typ „Tiles“

  - Zuordnung der Tiles-Kategorien (Sicherheit, Beleuchtung)
  - Behebung eines Fehlers bei der Ein-/Aus-Schaltfläche \* Hinzufügen von Informationen zum Protokoll im Debug-Modus
  - Ersetzen von ' im Namen des Geräts oder des Befehls durch ein Leerzeichen
  - Ersetzen des Buchstabens „É“ im Namen der Befehle durch „E“
    - Ausblenden der Schaltfläche „Befehl hinzufügen“
    - Hinzufügen von Generik-Typen zu bestimmten Befehlen
    - Änderung der Standard-Sichtbarkeit bestimmter Befehle (Akku, PIN-Code => nicht sichtbar)
    - Behebung des Problems, dass der Befehl „Suchen“ im Gerät „Home Adapter“ nach einer ersten Suche nicht angezeigt wurde \* Umbenennung von Befehlen (Hinzufügen des Status, falls der Befehl und die Info denselben Namen tragen)
      > Um alle Neuigkeiten zu den Geräten zu sehen, müssen Sie diese zunächst löschen und anschließend auf „Tiles suchen“ klicken.

- Befehl „refresh“ hinzugefügt => Befehl ist standardmäßig in den Befehlslisten ausgeblendet
- Sauberer Code

### 27/05/2020

- Zusätzliche Informationen bei der Suche nach Tiles
- Verbesserung der Anzeige der Befehle
- Migration der WLAN-API-Steuerung von V3 auf V5
- Trennung der Home- und Tiles-Geräte in der Geräteliste
- Bereinigung der Cron-Einträge beim Entfernen des Plugins

### 03/04/2020

- Trennung des Plugins und seiner Dokumentation

## 2019

### 19/12/2019

- Fehlerbehebung: Syntaxfehler

### 11/12/2019

- Bugfix: Abmeldung bei falscher Antwort
- Entfernen von Netzwerkgeräten bei ungültiger Antwort

### 10/12/2019

- Umstrukturierung der API-Klasse
- Einrichtung eines Cron-Jobs zur Aktualisierung des Tokens, um nur eine einzige Sitzung zu haben
- Aktualisierung des Netzwerk-Widgets

### 27/11/2019

- Hinzufügen von Widgets für den mobilen Bereich
