---
layout: default
title:  METAR/TAF Infos Météo Aéroports - Changelog BETA
lang: fr_FR
pluginId: Metar_infos
---

<img src="{{site.baseurl}}/plugin-Metar_infos/{{site.img}}/Metar_infos_icon.png" class="pluginLogo" width="100" />

## Important

> Ce changelog est hébergé provisoirement en attendant la remise en service du site officiel
>
> **_Pour rappel_** s'il n'y a pas d'information sur la mise à jour, c'est que celle-ci concerne uniquement de la mise à jour de documentation, de traduction ou de corrections de bugs mineurs.

## Changelog BETA

### 2024

#### 12/11/2024

- Correction max de la commande "Direction du Vent (degré)"

#### 04/11/2024

- Amélioration messages vocaux [https://community.jeedom.com/t/bug-humidite/133056?u=jag](https://community.jeedom.com/t/bug-humidite/133056?u=jag)

#### 03/11/2024

- Amélioration messages vocaux [https://community.jeedom.com/t/bug-humidite/133056?u=jag](https://community.jeedom.com/t/bug-humidite/133056?u=jag)
- Correction de bug refresh équipement merci @jpty

#### 01/11/2024

- Correction min/max humidité [https://community.jeedom.com/t/bug-humidite/133056?u=jag](https://community.jeedom.com/t/bug-humidite/133056?u=jag)
- Correction convertion vitesse du vent
- Suppression des parenthèses sur les messages vocaux[https://community.jeedom.com/t/bug-humidite/133056/4?u=jag](https://community.jeedom.com/t/bug-humidite/133056/4?u=jag)
- Traduction en français de la date pour les commandes "Bulletin météo" et "Heure locale du télégramme"


#### 27/10/2024

- Amélioration du bulletin météo vocal [https://community.jeedom.com/t/demande-damelioration-de-ce-super-plugin/132881?u=jag](https://community.jeedom.com/t/demande-damelioration-de-ce-super-plugin/132881?u=jag)

#### 05/10/2024

- Ajout image FOG nécessaire pour le widget


#### 19-20-21/09/2024

- Correction des warning PHP 8
- Reprise des textes des prévisions
- Ajout des min/max/unité des commandes numériques
- Correction de bug merci @jpty [https://community.jeedom.com/t/error-debian-12-php8/127613?u=jag](https://community.jeedom.com/t/error-debian-12-php8/127613?u=jag)
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
