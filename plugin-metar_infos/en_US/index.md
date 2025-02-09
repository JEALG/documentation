# Plugin Metar Infos

<img src="{{site.baseurl}}/plugin-metar_infos/{{site.img}}/metar_infos_icon.png" class="pluginLogo" width="100" />

## Important

> Cette documentation est hébergé provisoirement en attendant la remise en service du site officiel

## Description

Plugin permetant de recevoir les observations météo des aéroports (METAR) ainsi que les prévisions (TAF)

Un METAR (officiellement METeorological Aerodrome Report1 mais parfois défini par METeorological Airport Report2) est un rapport d'observation (et non de prévision) météorologique pour l'aviation. 
Ce plugin vous permet de récupérer et décoder les informations METAR d'un aéroport. Dans sa version actuelle, les infos suivantes sont disponibles (mais les données dépendent directement de ce qui est transmis par l'aéroport choisi) : 

> - Etat du ciel
> - Bulletin météo détaillé
> - Metar Data
> - Metar Valide
> - Heure UTC du télégramme
> - Heure Locale du télégramme
> - Vitesse du vent
> - Direction du vent
> - Direction du vent(cap)
> - Visibilité
> - Température
> - Point de rosée
> - Humidité
> - Pression Atmosphérique
> - Nuages niveau 1 à 3
> - Altitude Nuages niveau 1 à 3

## Configuration

Le plugin ne comporte pas de configuration particulière.

> Dans l'équipement il faut choisir l'aéroport ou Saisir manuelle le code OACI 

<img src="../images/choix_aeroport.png" alt="Choix de l'Aéroport" width="900" />

> Type d'information : choisir le type de données soit METAR ou METAR et TAF

<img src="../images/choix_metar.png" alt="Choix de l'Aéroport" width="900" />
