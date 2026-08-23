# Freebox_OS-Plugin

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />


## Beschreibung

Mit diesem Plugin können Sie Informationen von Ihrem FreeboxOS (Freebox Révolution-, 4K-, DELTA-, POP- oder Ultra-Server) abrufen und über Widgets oder Szenarien, die die erstellten Befehle enthalten, mit diesem interagieren.

>
> **Damit das Plugin funktioniert, muss die Freebox Serveur in der Version 4.12.1 installiert sein.**

Die auf Jeedom verfügbaren Informationen zu Ihrem Freebox-Server sind:

- **Systeminformationen:**
  - WLAN ausschalten
  - Freebox neu starten
  - Internet-Übertragungsraten
  - Der Status Ihrer Verbindung
  - Verwaltung der Anruffilterung
- **Telefon:** in den letzten 24 Stunden
  - Die Anzahl der verpassten Anrufe
  - Die Anzahl der getätigten Anrufe
  - Die Anzahl der eingegangenen Anrufe
  - Anzahl der Sprachnachrichten
- **Festplatte:**
  - Der verfügbare Speicherplatz auf Ihren mit der Freebox Serveur verbundenen Festplatten.
- **Geräte, die mit dem LAN und dem Gast-WLAN verbunden sind:**
  - Der Status jedes DHCP-Geräts
  - Die Befehlsfunktion **_Wake on LAN_** kann nur im Rahmen eines Szenarios verwendet werden
- **Hausautomation (nur für das Modell DELTA):**
  - Ruft die Daten des vernetzten Hauses ab

## Installation und Konfiguration

Sobald das Plugin installiert und aktiviert ist, ist keine weitere Konfiguration erforderlich.

## Kopplung (Authentifizierung)

Gehen Sie auf die Hauptseite des Plugins und klicken Sie auf

<p><img src="../images/appairage.png" alt="Modales Fenster zum Koppeln" width="60" /></p>

Befolgen Sie anschließend die Anweisungen auf den verschiedenen Bildschirmen, um die Kopplung zu bestätigen

<p><img src="../images/freebox_os_screenshot2.png" alt="Authentifizierung 1" width="300" /></p>

### Einstellungen

Im folgenden Fenster können Sie folgende Einstellungen ändern:

- **IP-Adresse der Freebox**: Login-Adresse der Freebox _(Standard: maFreebox.Freebox.fr)_
- **Name des verbundenen Geräts**: Der Name des Jeedom (dieses Feld ist gesperrt)
- **Erkannte Geräte automatisch hinzufügen in:**: Standardraum angeben
- Sie können auf die Schaltfläche **Konfiguration zurücksetzen** klicken, um die Standardeinstellungen wiederherzustellen.
  > - Ruft den **Namen Ihres Jeedom** ab, falls sich dieser seit der letzten Kopplung geändert hat
  > - Setzt die folgenden Werte auf die Standardwerte zurück:
  >     - **API-Version der Freebox**: v10
  >     - **IP Freebox**: maFreebox.Freebox.fr
  >     - Löscht alle anderen Konfigurationen des Plugins

- Vergessen Sie nicht, nach Ihren Änderungen auf **Speichern** zu klicken

> Es ist unbedingt erforderlich, dass Ihr Jeedom einen Namen hat, damit die Kopplung des Plugins mit Ihrer Freebox fortgesetzt werden kann.

<p><img src="../images/freebox_os_screenshot3.png" alt="Authentifizierung 2" width="300" /></p>

### Authentifizierung

#### Mindest-Firmware-Version der Freebox

 > Damit das Plugin funktioniert, ist eine bestimmte Mindestversion der Firmware erforderlich.
 > Die erforderliche Firmware-Version ist im Changelog am Anfang sowie am Anfang dieser Dokumentation angegeben.

#### Authentifizierung

Im folgenden Fenster wird die Authentifizierung auf der Freebox durchgeführt

- Klicken Sie auf die Schaltfläche **Authentifizierung starten**
- Behalten Sie sowohl die Anmeldungen auf diesem Bildschirm als auch auf der Freebox im Auge

<p><img src="../images/freebox_os_screenshot4.png" alt="Authentifizierung 3" width="300" /></p>

### Berechtigungsprüfung

Im folgenden Fenster überprüft das System die der Anwendung zugewiesenen Rechte

- Informationen zum Ändern der Zugriffsrechte auf der Freebox finden Sie im Abschnitt „Zugriffsrechte“ (in dieser Dokumentation).
- Sobald die Berechtigungen festgelegt sind, klicken Sie auf die Schaltfläche **Berechtigungen prüfen**.
  > Wenn die Berechtigungen in Ordnung sind, wird die Schaltfläche **Weiter** sichtbar.
  > Die Pflichtangaben sind fett gedruckt

<p><img src="../images/freebox_os_screenshot5.png" alt="Authentifizierung 4" width="300" /></p>

### Freebox-Komponenten mit Jeedom-Objekten verknüpfen

> Dieses Fenster wird nur angezeigt, wenn es sich bei der Freebox um ein DELTA-Modell handelt.
>
> Der Cron-Job „Globale Aktualisierung der Kacheln“ kann aktiviert oder deaktiviert werden.
>
> <b>Vergessen Sie nicht</b>, auf „Speichern“ zu klicken, damit die Änderungen übernommen werden

<p><img src="../images/freebox_os_screenshot6.png" alt="Authentifizierung 4" width="300" /></p>

### Scannen

Im folgenden Fenster können Sie den Scan der verschiedenen Geräte starten.

<p><img src="../images/freebox_os_screenshot7.png" alt="Authentifizierung 5" width="300" /></p>

### Authentifizierung abgeschlossen

Die Authentifizierung war erfolgreich.

<p><img src="../images/freebox_os_screenshot8.png" alt="Authentifizierung 6" width="300" /></p>

### Problem bei der Authentifizierung behoben

Bei Problemen mit der Authentifizierung müssen die Logs des Plugins im Debug-Modus bereitgestellt werden
Hier ein Beispiel
```
000|[2024-10-11 18:53:49] INFO  ──────────▶︎ Étape : setting
0001|[2024-10-11 18:53:49] INFO  ───▶︎ IP : mafreebox.freebox.fr
0002|[2024-10-11 18:53:49] INFO  ───▶︎ Nom API : Plugin Freebox OS
0003|[2024-10-11 18:53:49] INFO  ───▶︎ Id API : plugin.freebox.jeedom
0004|[2024-10-11 18:53:49] INFO  ───▶︎ Nom de votre Jeedom : JAG Jeedom-VM2
0005|[2024-10-11 18:53:49] INFO  ───▶︎ Objet par défaut : 13
0006|[2024-10-11 18:53:49] INFO  ───▶︎ Version API Freebox : v12
0007|[2024-10-11 18:53:51] INFO  ──────────▶︎ Étape : authentification
0008|[2024-10-11 18:53:53] INFO  ──────────▶︎ Étape : rights
0009|[2024-10-11 18:53:57] DEBUG  OK  Close Session
0010|[2024-10-11 18:53:57] DEBUG  [Freebox Close Session] : {"uid":"","success":false,"msg":"Vous devez vous connecter pour accéder à cette fonction","result":{"password_salt":"","challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr"},"error_code":"invalid_session"}
0011|[2024-10-11 18:53:57] DEBUG  [Freebox Password] : {"success":true,"result":{"logged_in":false,"challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr","password_salt":"","password_set":true}}
0012|[2024-10-11 18:53:57] DEBUG  [get Freebox Open Session Data] : {"result":{"session_token":"eRDFtl35L8ENEND2UGlooFzLhAgmv8CGPbMLiegdyC2n4z3DDr4UEYY+zYMOhSkS","challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr","password_salt":"P","permissions":{"parental":true,"contacts":true,"explorer":true,"tv":true,"wdo":true,"downloader":true,"profile":true,"camera":true,"settings":true,"calls":true,"home":true,"pvr":true,"vm":true,"player":true},"password_set":true},"success":true}
0013|[2024-10-11 18:53:57] INFO  ───▶︎ Les droits sont OK
0014|[2024-10-11 18:53:58] INFO  ──────────▶︎ Étape : room
0015|[2024-10-11 18:53:58] INFO  ───▶︎ Cron Global Titles ACTIVATION : NOK
0016|[2024-10-11 18:53:58] INFO  ───▶︎ Compatibilité avec la partie domotique : NOK
0017|[2024-10-11 18:53:58] INFO  ──────────▶︎ Étape : scan
0018|[2024-10-11 18:53:59] INFO  ──────────▶︎ Étape : end
```

<p><img src="../images/debug_log.png" alt="Aktivierung des Debug-Protokolls" width="300" /></p>


## Zugriffsrechte

Für die Nutzung des Plugins sind bestimmte zusätzliche Zugriffsrechte erforderlich; diese müssen **unbedingt direkt über das Betriebssystem der Freebox zugewiesen und geändert werden**

- Sich bei der Freebox-Benutzeroberfläche anmelden (http://maFreebox.Freebox.fr)
- Einstellungen der Freebox öffnen

<p><img src="../images/freebox_para.png" alt="Freebox-Einstellungen" width="100" /></p>

- Öffnen Sie die Zugriffsverwaltung der Freebox _(diese Einstellung finden Sie im erweiterten Modus)_

<p><img src="../images/freebox_gestion_acces_1.png" alt="Einstellungen für die Zugriffsverwaltung der Freebox" width="600" /></p>

- Klicken Sie auf die Registerkarte **Anwendungen**
- Wählen Sie in der Liste die App aus, die bei der Installation des Plugins angegeben wurde _(Standard: Freebox OS-Plugin)_

<p><img src="../images/freebox_gestion_acces_2.png" alt="Einstellungen für die Zugriffsverwaltung der Freebox" width="500" /></p>

- **Alle Zugriffsrechte gewähren**

<p><img src="../images/modification_droit.png" alt="Änderung spezifischer Zugriffsrechte" width="500" /></p>

# Standardausstattung

Klicken Sie auf die Schaltfläche **_Standardgeräte scannen_**. Das Plugin erstellt daraufhin die verschiedenen Standardgeräte der Freebox.

<p><img src="../images/recherche_systeme.png" alt="Suche nach Systemkomponenten" width="60" /></p>

Die folgenden Geräte und Steuerungen werden angelegt:

- **LCD-Display**
  - Helligkeitseinstellung
  - Einstellung der Textausrichtung
  - WLAN-Schlüssel verbergen
  - Steuerung von Lichtbändern (sofern die Box kompatibel ist)
  - LED ausschalten (sofern die Box kompatibel ist)
- **Air Média**
  - Auswahl des aktuellen Players
  - AirMedia Start/Stopp
- **Verbundene Geräte** und **Geräte mit Gast-WLAN-Zugang**
  - Alle an die Freebox angeschlossenen Geräte
  - Möglichkeit zur Verwendung des Befehls **_Wake on LAN_** (nur im Rahmen eines Szenarios)
- **Festplatte**
  - Festplattenspeicherbelegung
  - Temperatur
  - RAID-Typ (nur für kompatible Freebox-Geräte)
- **Freebox-Übertragungsraten**
  - Freebox: Download-Geschwindigkeit, Upload-Geschwindigkeit, Bandbreite (Download), Bandbreite (Upload)
  - Freebox Media
  - Freebox-Status
  - Verbindungstyp
  - Verbindungsstatus
  - IP
  - Antwort auf den Ping
- **Player**
  - Mac
  - Typ
  - Modell
  - Version
  - API verfügbar
  - Im Netzwerk verfügbar
  - Status (ein oder aus)
    > Der Befehl wird nur erstellt, wenn der Player seinen Status zurückgibt und über eine ID verfügt.
    > **Der Player muss während der Suche unbedingt eingeschaltet sein und darf sich nicht im Ruhemodus (Révolution) befinden.**
    > Die Player mini4K/POP sind verfügbar, melden jedoch keinen Status zurück
- **Dateifreigabe zwischen Windows und Mac**
  - Dateifreigabe unter Mac, Windows und FTP aktivieren/deaktivieren
  - Druckerfreigabe aktivieren/deaktivieren (nur verfügbar, wenn SMBv2 nicht aktiv ist)
- **System**
  - Update
  - Neustart
  - Freebox-Firmware-Version
  - Mac
  - IP v4/v6
  - Lüftergeschwindigkeit
  - Temperaturen _(Temp Sw, Temp Cpub, Temp Cpum)_
  - Eingeschaltet seit
  - Board-Name
  - seriell
  - 4G, sofern die Karte in der Freebox steckt
- **Telefon** in den letzten 24 Stunden
  - Anzahl der verpassten / empfangenen / getätigten Anrufe
  - Liste der verpassten / empfangenen / getätigten Anrufe
  - Anzahl der Sprachnachrichten
  - Liste der abgehörten und neuen Sprachnachrichten
- **Downloads**
  - Anzahl der Aufgaben
  - Anzahl der aktiven, im Abruf befindlichen, in Bearbeitung befindlichen, in Überprüfung befindlichen, ausstehenden, fehlerhaften, angehaltenen und abgeschlossenen Aufgaben sowie der RSS-Feeds und ungelesenen RSS-Feeds
  - Download läuft
  - Empfangs- und Sendegeschwindigkeit
  - Start, Stopp
  - Download-Modus
  - Planungsstand
  - Anmeldestatus
- **VM** (nur für kompatible Freebox-Geräte)
  - Status
  - Mögliche Aktionen: Stopp, Neustart, Start
  - Info: Anzahl der CPUs, MAC-Adresse, Arbeitsspeicher, USB-Anschluss, virtueller Bildschirm, Festplattentyp
- **WLAN**
  - WLAN-Status
  - WLAN ein/aus
  - Verwaltung der Anruffilterung
  - Planungsstand
  - WPS-Sitzung EIN/AUS
  - Schwarze Liste für Mac
  - Weiße Mac-Liste
  - Status der WLAN-Karte

## Kindersicherung

Klicken Sie auf die Schaltfläche **_Kindersicherung scannen_**. Das Plugin erstellt daraufhin die verschiedenen Systemkomponenten der Freebox.

> Diese Steuerungsfunktionen wurden mit Version 4.2 der Freebox eingeführt.

<p><img src="../images/recherche_parental.png" alt="Suche nach Kindersicherungen" width="60" /></p>

- Die folgenden Geräte und Steuerungen werden angelegt:
  
  > - Status
  > - Blockieren
  > - Zulassen
  > - 30 Min./1 Std./2 Std. sperren

## Besonderheiten von Home Adapters (nur Freebox Delta), vernetzte Geräte, Festplatte und System

Diese vier Geräte sind bei ihrer Erstellung standardmäßig leer, mit Ausnahme des Systems, das die für alle Freebox-Geräte gemeinsamen Informationen enthält.

Öffnen Sie jedes Gerät und klicken Sie auf die Schaltfläche „Suchen“

> Das Plugin sucht nach den verschiedenen zugehörigen Befehlen und erstellt diese.

<p><img src="../images/recherche_commandes.png" alt="Suche nach bestimmten Geräten" width="800" /></p>

> Ein täglicher Cron-Job sorgt dafür, dass automatisch nach neuen Geräten gesucht wird

## Netzwerkverwaltung

Mit dieser Anlage können Sie:

> - Eine feste IP-Adresse zuweisen
> - Verwaltung der MAC-Adressfilterung
> - Wake-on-LAN-Funktion
> - Gerätetyp ändern

### IP-Adresse zuweisen

<p><img src="../images/modif__equip_ip_fixe.png" alt="IP-Änderung" width="800" /></p>

Die folgenden Felder müssen ausgefüllt sein

- Verbundenes Gerät auswählen
- Auswahl ändern Gerät mit dem nächsten Wert

  > - **Feste IP-Adresse hinzufügen**
  > - **Feste IP-Adresse löschen**
  > - **IP-Adresse des Geräts ändern**

Das geht auch mit dem Befehl
   > - **Gerätetyp / IP ändern**

- IP-Auswahl: Geben Sie die IP-Adresse des Geräts an
- Gerätenamen auswählen: Geben Sie den Namen des Geräts ein

  > Wenn das Feld „Name“ leer ist, übernimmt das Plugin den in der Freebox hinterlegten Gerätenamen.

- Kommentare: Hier können Sie einen Kommentar eingeben (optional)

### Gerätetyp ändern

<p><img src="../images/modif__equip_type.png" alt="Änderung der Geräte" width="800" /></p>

Die folgenden Felder müssen ausgefüllt sein

- Verbundenes Gerät auswählen
- Auswahl ändern Gerät mit dem nächsten Wert

  > - **Gerätetyp / IP ändern**

- Auswahl „Gerätetyp“: Wählen Sie den Gerätetyp aus

  > Wenn das Feld „Name“ leer ist, übernimmt das Plugin den in der Freebox hinterlegten Gerätenamen.
  
- Kommentare: Hier können Sie einen Kommentar eingeben
- Gerät bearbeiten: Ermöglicht es, die Änderung an die Freebox zu senden

### Verwaltung der MAC-Adressfilterung (WLAN)

<p><img src="../images/modif__equip_filtrage.png" alt="Änderung der Geräte" width="800" /></p>

Dies ist über Befehle von den angeschlossenen Geräten oder über WLAN möglich.
Die folgenden Felder müssen ausgefüllt sein

- Verbundenes Gerät auswählen
- Auswahl ändern Gerät mit dem nächsten Wert

  > - **Blacklist hinzufügen/bearbeiten**
  > - **Whitelist hinzufügen/bearbeiten**
  > - **Schwarze/Weiße Liste löschen**

- Kommentare: Hier können Sie einen Kommentar oder ein Passwort eingeben
- Gerät bearbeiten: Ermöglicht es, die Änderung an die Freebox zu senden

### Wake-on-LAN-Funktion

<p><img src="../images/modif__equip_wol.png" alt="Änderung der Geräte" width="800" /></p>

- Verbundenes Gerät auswählen
- Auswahl ändern Gerät mit dem nächsten Wert

  > - **Wake-on-LAN**

- Anmerkungen: Ermöglicht die Eingabe eines Passworts
- Gerät bearbeiten: Ermöglicht es, die Änderung an die Freebox zu senden

Die Steuerung erfolgt über das Modul „Verbundene Geräte“ oder über ein Szenario.

## Freebox Delta

> Die Freebox Delta bietet ein Sicherheitspaket sowie die Anbindung an bestimmte Geräte.

Klicken Sie auf die Schaltfläche **_Scan Tiles_**. Daraufhin werden die Geräte und die Steuerelemente der verschiedenen angeschlossenen Geräte angelegt.

<p><img src="../images/recherche_tiles.png" alt="Suche nach spezifischen Freebox-Delta-Geräten" width="60" /></p>

### Alarmstatus

> Das Plugin meldet den Alarmstatus über den Befehl „Alarmstatus“

![Alarmstatus](../images/alarme_statut.png)
Mögliche Werte sind:

> **idle** = Alarm deaktiviert
> **alarm_1_arming** = Der Hauptalarm ist aktiviert. Es handelt sich um einen Countdown, bei dem nur Sensoren, die sich nicht im Bereich befinden, den Alarm auslösen können.
> **alarm_2_arming** = Die Teilalarmfunktion ist aktiviert. Es handelt sich um einen Countdown, bei dem nur Sensoren, die sich nicht im Überwachungsbereich befinden, den Alarm auslösen können.
> **alarm_1_armed** = Vollalarm aktiviert
> **alarm_2_armed** = Teilalarm aktiviert
> **alarm1_alert_timer** = Der Hauptalarm wurde durch einen Sensor in der Zeitzone ausgelöst, und die Sirene wird nach Ablauf eines Countdowns ertönen
> **alarm2_alert_timer** = Der Nachtalarm wurde durch einen Sensor in der Zeitzone ausgelöst, und die Sirene wird nach Ablauf eines Countdowns ertönen
> **Alarm** = Die Sirene ertönt

> Das Alarmsystem ist mit Homebridge und der mobilen App kompatibel: Es sind keine Einstellungen erforderlich.
> Um die Integration zu ermöglichen, wurden Informationsbefehle hinzugefügt, die die Interaktion mit dem Alarm-Plugin ermöglichen.
>
> - **Aktiv** = Binärinformation (1 = Alarm aktiviert)
> - **Status** = Binäre Information (1 = Sirene aktiv)

<p><img src="../images/alarme_dashboard.png" alt="Alarmstatus" width="250" /></p>

### Status der Fernbedienung

> Das Plugin protokolliert den Verlauf der Fernbedienung und zeigt die zuletzt mit der Fernbedienung ausgeführte Aktion an.

- Mögliche Werte sind:
  > **null** oder **0** = Kein Status
  > **1** = Hauptalarm
  > **2** = Deaktivierung
  > **3** = Sekundärer Alarm

### Kameras

> Die Kameras werden automatisch erstellt, wenn das Kamera-Plugin installiert ist

## Aktualisierungsintervall (Cron) der Geräte

- Es ist möglich, den Cron-Zeitplan für die Aktualisierung jedes Geräts zu ändern. Standardmäßig gilt:

  > Home Adapter, FREEBOX – Fernbedienung (Alarmanlage), Kindersicherung und „Meine Geräte“ (außer Festplatte) = **Cron wird auf 5 Minuten eingestellt**
  >
  > Festplatte = **Cron wird auf 1 Uhr eingestellt**

- Mit diesem Cron-Job können verschiedene Befehle vom Typ „Infos“ aktualisiert werden; die Geräte werden automatisch aktualisiert, sobald ein Befehl ausgeführt wird.
  > Aktionsbefehle sind von diesem Cron-Job nicht betroffen.
  >
  > Je kürzer die Zeit ist, desto höher ist die Auslastung der Freebox-CPU.

- Seit der Plugin-Version 20210507 gilt für den **Bereich Hausautomation**
  > Ein globaler Aktualisierungs-Cron-Job ist standardmäßig aktiviert
  >
  > <p><img src="../images/cron_tiles.png" alt="Aktualisierungszeit" width="800" /></p>
  >
  > Wenn diese Option deaktiviert ist, wird der **Cron auf 1 Minute eingestellt**

## Die Kacheln

*Aufgrund der Weiterentwicklung der Freebox*S sind möglicherweise nicht alle Geräte in das System integriert.*

- Um die neuen Systeme integrieren zu können, ist Folgendes erforderlich:

  > Das Plugin in den Debug-Modus versetzen
  > Den Daemon neu starten
  > **_Debug Tiles_** erstellen

<p><img src="../images/debug.png" alt="Debug-Kacheln" width="60" /></p>

Eröffnen Sie ein Thema (sofern noch kein Thema diese Anfrage behandelt) in der Community und geben Sie folgende Informationen an

- Einen Screenshot der Anlage erstellen

<p><img src="../images/tiles1.png" alt="Ausstattung Tiles 1" width="800" /></p>

- Einen Screenshot der Steuerelemente des Geräts erstellen

<p><img src="../images/tiles2.png" alt="Ausstattung Tiles 2" width="800" /></p>

- Bitte reichen Sie die Protokolle im Textformat ein und nicht als Screenshot.
  > [Siehe Absatz **11**: Richtig formatieren](https://community.jeedom.com/t/comment-nous-aider-a-vous-aider-ou-comment-poser-une-bonne-question/34932)

```
    [2020-08-24 07:37:41][DEBUG] : ┌───────── Commande trouvée pour l'équipement FREEBOX : FREEBOX - Eclairage Canapé -- Pièce : Salon (Node ID 9)
[2020-08-24 07:37:41][DEBUG] : │ Label : Enclenché -- Name : switch_state
[2020-08-24 07:37:41][DEBUG] : │ Type (eq) : light -- Action (eq): intensity_picker
[2020-08-24 07:37:41][DEBUG] : │ Index : 0 -- Value Type : bool -- Access : rw
[2020-08-24 07:37:41][DEBUG] : │ Valeur actuelle :
[2020-08-24 07:37:41][DEBUG] : │ Range : ----- -- Range color : -
[2020-08-24 07:37:41][DEBUG] : │ Name: Etat -- Type : info -- LogicalID : 0 -- Template Widget / Ligne : core::light/0-- Type de générique : LIGHT_STATE -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : │ No Repeat pour l'info avec le nom : Etat
[2020-08-24 07:37:41][DEBUG] : │ Name: On -- Type : action -- LogicalID : PB_On -- Template Widget / Ligne : core::light/1-- Type de générique : LIGHT_ON -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : │ Name: Off -- Type : action -- LogicalID : PB_Off -- Template Widget / Ligne : core::light/0-- Type de générique : LIGHT_OFF -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : └─────────
[2020-08-24 07:37:41][DEBUG] : ┌───────── Commande trouvée pour l'équipement FREEBOX : FREEBOX - Eclairage Canapé -- Pièce : Salon (Node ID 9)
[2020-08-24 07:37:41][DEBUG] : │ Label : Luminosité -- Name : luminosity
[2020-08-24 07:37:41][DEBUG] : │ Type (eq) : light -- Action (eq): intensity_picker
[2020-08-24 07:37:41][DEBUG] : │ Index : 2 -- Value Type : int -- Access : rw
[2020-08-24 07:37:41][DEBUG] : │ Valeur actuelle : 254
[2020-08-24 07:37:41][DEBUG] : │ Range : ----- -- Range color : -
[2020-08-24 07:37:41][DEBUG] : │ Name: Etat Luminosité -- Type : info -- LogicalID : 2 -- Template Widget / Ligne : /0-- Type de générique : LIGHT_COLOR -- Inverser : 0 -- Icône :  -- Min/Max : 0/255
[2020-08-24 07:37:41][DEBUG] : │ No Repeat pour l'info avec le nom : Etat Luminosité
[2020-08-24 07:37:41][DEBUG] : │ Name: Luminosité -- Type : action -- LogicalID : 2 -- Template Widget / Ligne : default/0-- Type de générique : LIGHT_SET_COLOR -- Inverser : 0 -- Icône :  -- Min/Max : 0/255
[2020-08-24 07:37:41][DEBUG] : └─────────
```
