---
layout: default
title:  Changelog-BETA
lang: fr_FR
pluginId: Metar_infos
---

<img src="{{site.baseurl}}/plugin-metar_infos/{{site.img}}/metar_infos_icon.png" class="pluginLogo" width="100" />

## Important

> Ce changelog est hébergé provisoirement en attendant la remise en service du site officiel
>
> **_Pour rappel_** s'il n'y a pas d'information sur la mise à jour, c'est que celle-ci concerne uniquement de la mise à jour de documentation, de traduction ou de corrections de bugs mineurs.

## Changelog BETA

### 2025

#### 19/01/2025

- Amélioration log pour les problèmes de téléchargement des données
- Contrôle TAF Valide avant de faire les mises à jour des données TAF

### 2024

#### 28/12/2024

- Amélioration log
- Mise à jour icône plugin
- Mise à jour screen pour le market

#### 25/11/2024

- Conversion des rafales de vent en km/h
- Ajout rafales de vent pour les nouveaux équipements (Pour les anciens équipements, il suffit d'enregistrer celui-ci)
- Ajout Widget mobile sur la commande "Icône météo"
- Ajout icône pour la commande point de rosée

#### 22/11/2024

- Ajout image neige pour le widget

#### 13/11/2024

- Remplacement du widget "Badge" par le widget "Line" (cela s'applique uniquement sur les nouveaux équipements) [https://community.jeedom.com/t/affichage-nouveau-plugin-metar-infos-sur-mobile/133685](https://community.jeedom.com/t/affichage-nouveau-plugin-metar-infos-sur-mobile/133685)

#### 12/11/2024

- Correction max de la commande "Direction du Vent (degré)"

#### 04/11/2024

- Amélioration messages vocaux [https://community.jeedom.com/t/bug-humidite/133056](https://community.jeedom.com/t/bug-humidite/133056)

#### 03/11/2024

- Amélioration messages vocaux [https://community.jeedom.com/t/bug-humidite/133056](https://community.jeedom.com/t/bug-humidite/133056)
- Correction de bug refresh équipement merci @jpty

#### 01/11/2024

- Correction min/max humidité [https://community.jeedom.com/t/bug-humidite/133056](https://community.jeedom.com/t/bug-humidite/133056)
- Correction convertion vitesse du vent
- Suppression des parenthèses sur les messages vocaux[https://community.jeedom.com/t/bug-humidite/133056/4](https://community.jeedom.com/t/bug-humidite/133056/4)
- Traduction en français de la date pour les commandes "Bulletin météo" et "Heure locale du télégramme"


#### 27/10/2024

- Amélioration du bulletin météo vocal [https://community.jeedom.com/t/demande-damelioration-de-ce-super-plugin/132881](https://community.jeedom.com/t/demande-damelioration-de-ce-super-plugin/132881)

#### 05/10/2024

- Ajout image FOG nécessaire pour le widget


#### 19-20-21/09/2024

- Correction des warning PHP 8
- Reprise des textes des prévisions
- Ajout des min/max/unité des commandes numériques
- Correction de bug merci @jpty [https://community.jeedom.com/t/error-debian-12-php8/127613](https://community.jeedom.com/t/error-debian-12-php8/127613)
- Nettoyage du code
- Ajout des traductions
- Correction des crons
- Mise à jour des noms des commandes (Update + Nouveau) => Intégration traduction
- Ajout commande "icône météo" => Merci @Phpvarious + ajout widget
- Suppression commande tendance
- Mise à jour code ICAO (typo)
- Reprise de l'ensemble des mises à jours des commandes => Merci @Phpvarious
- Amélioration des logs
- Changement du logicalId pour la commande "TAF valide" de "TAFvalide" à "tafvalide"

> **Attention : Il faut enregistrer les équipements pour avoir les dernières corrections ou ajout de commande.**
>
> **Version mini du Core V4.3**
