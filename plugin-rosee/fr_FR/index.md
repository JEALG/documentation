---
layout: default
title: Plugin Rosee - documentation
lang: fr_FR
pluginId: rosee
---

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

# Description

Ce plugin permet d'obtenir le point de rosée pour savoir si l'herbe sera mouillée le matin, ou bien en hiver savoir s'il va falloir gratter le pare-brise.
Pour fonctionner, on doit indiquer un équipement température et un équipement humidité (extérieures, bien sûr…).
Il est aussi possible de calculer la tendance Météo à venir en se basant sur l'évolution de la météo.

# Configuration

Le plugin ne comporte pas de configuration générale, il faut :

> Choisir une méthode de calcul :

    - Humidité absolue
    - Point de Givre
    - Point de Rosée
    - Point de Rosée et Point de Givre
    - Tendance Météo
    - Températures ressenties

> Renseigner les champs obligatoires suivant la méthode de calcul :

    - Équipement "Température" (°C)
    - Équipement "Humidité Relative" (%)
    - Équipement "Vitesse du Vent"
    - Équipement "Pression Atmosphérique" (hPa) : Ce champ est obligatoire pour la méthode de calcul "Tendance Météo" et il doit avoir l'historique d'activé. Pour les autres calculs, la valeur est fixée à 1013.25 hPa si non renseignée.

<b>En option : </b>

> - Seuil de l'Alerte Rosée (°C) : Seuil de déclenchement de l'alerte rosée, 2°C par défaut (dépression du point de rosée T°-Tr°). A ajuster en fonction des observations locales.
> - Seuil d'humidité absolue : Seuil humidité absolue en dessous duquel il est peu probable qu'il givre, 2.8 par défaut.
> - Offset Température : A ajuster en fonction des observations locales et de la position de la sonde, 0 par défaut.

# Alerte Givre

> Sources :
>
> - <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/</a>

Le plugin calcule 4 niveaux d'alerte :

|  Cas  | Infos                                                                                                                                                                                                                                                         |
| :---: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **0** | - Calcul : Aucun cas ci-dessous couvert<br/>- Alerte Givre : 0<br/>- Alerte Rosée : Automatique<br/>- Message numérique Givre : 0<br/>- Message d'info : Aucun risque de Givrage                                                                              |
| **1** | - Calcul : (Température <=1 et Point de Givrage <= 0) et (Humidité absolue en (gr/m3) < Seuil d'humidité absolue)<br/>- Alerte Givre : 1<br/>- Alerte Rosée : forcée à 0<br/>- Message numérique : 1<br/>- Message : Givre peu probable malgré la température |
| **2** | - Calcul : (Température <=4 et Point de Givrage <= 0.5)<br/>- Alerte Givre : 1<br/>- Alerte Rosée : forcée à 0<br/>- Message numérique : 2<br/>- Message : Risque de givre                                                                                    |
| **3** | - Calcul : (Température <=1 et Point de Givrage <= 0) et (Humidité absolue en (gr/m3) > Seuil d'humidité absolue)<br/>- Alerte Givre : 1<br/>- Alerte Rosée : forcée à 0<br/>- Message numérique : 3<br/>- Message : Givre, Présence de givre                 |

# Tendance Météo

> Sources :
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

Le plugin calcule 6 niveaux d'information :

|  Niveau  | Tendance                           |                             Image du widget                              |
| :------: | :--------------------------------- | :----------------------------------------------------------------------: |
| <b>0</b> | Forte dégradation, instable        | <img src="../{{site.img}}/tendance_0.png" alt="Tendance 0" width="40" /> |
| <b>1</b> | Dégradation, mauvais temps durable | <img src="../{{site.img}}/tendance_1.png" alt="Tendance 1" width="40" /> |
| <b>2</b> | Lente dégradation, temps stable    | <img src="../{{site.img}}/tendance_2.png" alt="Tendance 2" width="40" /> |
| <b>3</b> | Lente amélioration, temps stable   | <img src="../{{site.img}}/tendance_3.png" alt="Tendance 3" width="40" /> |
| <b>4</b> | Amélioration, beau temps durable   | <img src="../{{site.img}}/tendance_4.png" alt="Tendance 4" width="40" /> |
| <b>5</b> | Forte embellie, instable           | <img src="../{{site.img}}/tendance_5.png" alt="Tendance 5" width="40" /> |

Le plugin met à disposition deux widgets pour la tendance :

> - Rosée/Tendance (Icône 40x40) (Widget par défaut)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Rosée/Tendance 80x80 (Icône 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>

# Températures ressenties

> Sources :
>
> - <a href="https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul">https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul</a>
> - <a href="http://www.meteo-mussidan.fr/hum.php">http://www.meteo-mussidan.fr/hum.php</a>

| Message numérique | Message                                                                                                            |
| :---------------: | :----------------------------------------------------------------------------------------------------------------- |
|     <b>-7</b>     | Danger ! Risque extrêmement élevé de gelures en moins de 2 minutes (voir note) et d\'hypothermie. Rester à l\'abri |
|     <b>-6</b>     | Risque très élevé de gelures en 2 à 5 minutes (voir note) sans protection intégrale ni activité                    |
|     <b>-5</b>     | Risque élevé de gelures en 5 à 10 minutes (voir note) de la peau exposée et d’hypothermie                          |
|     <b>-4</b>     | Risque modéré de gelures en 10 à 30 minutes de la peau exposée et d’hypothermie'                                   |
|     <b>-3</b>     | Faible risque de gelures et d’hypothermie                                                                          |
|     <b>-2</b>     | Faible risque de gelures                                                                                           |
|     <b>-1</b>     | Pas de risque de gelures ni d’hypothermie (pour une exposition normale)                                            |
|     <b>1</b>      | Sensation de frais ou de froid                                                                                     |
|     <b>2</b>      | Aucun inconfort                                                                                                    |
|     <b>3</b>      | Sensation de bien être                                                                                             |
|     <b>4</b>      | Sensation d'inconfort plus ou moins grande                                                                         |
|     <b>5</b>      | Sensation d'inconfort assez grande. Prudence. Ralentir certaines activités en plein air.                           |
|     <b>6</b>      | Sensation d'inconfort généralisée. Danger. Éviter les efforts.                                                     |
|     <b>7</b>      | Danger extrême. Arrêt de travail dans de nombreux domaines.                                                        |
|     <b>8</b>      | Coup de chaleur imminent (danger de mort).                                                                         |

- **Est-ce que le plugin s'appuie sur des API tiers ?**

> Non, le plugin fait le calcul en interne par rapport à la température, l’humidité et la vitesse du vent

- **Refroidissement éolien (ou indice Windchill), kesako ?**

> Le refroidissement éolien, parfois aussi appelé facteur vent, ou windchill désigne la sensation de froid produite par le vent, alors que la température réelle de l'air ambiant ne s'abaisse pas.

- **Et l'indice de chaleur ou humidex ?**

> L’indice de chaleur (nom original en anglais Heat Index (HI) ou humiture) est un indice développé aux États-Unis.
>
> Il combine la température de l'air ambiant et l'humidité relative, dans des zones ombragées, pour tenter de déterminer la perception de la température que ressent le corps humain, c'est-à-dire de combien il ressentirait la chaleur si l'hygrométrie était à une autre valeur à l'ombre.
>
> Le résultat est également connu comme la _"température ressentie à l'air"_ ou _"la température apparente"_.
>
> Par exemple, quand la température est de 32°C (ou 90°F) avec 70 % d'humidité relative :
>
> - L'index de chaleur est alors de 41°C (ou 106°F).
> - Cette température d'index de chaleur a une humidité implicite (non spécifiée) de 20 %.
> - C'est la valeur de l'humidité relative pour laquelle la formule d'index de chaleur indique que 41°C est ressentie comme 41 °C.
> - Une température d'index de chaleur de 32°C a une humidité relative implicite de 38 %.
>
> L’indice de chaleur est basé sur la capacité du corps humain à refroidir la peau par la production de sueur.
>
> Celle-ci s'évapore dans l'air ce qui nécessite de l'énergie qui est prise au milieu et baisse la température de la couche limite touchant à la peau, donnant une sensation de fraîcheur.
>
> En augmentant, l'humidité relative de l'air, l'évaporation se fait moins bien et donne une sensation subjective de chaleur accrue. Cet indice ne doit pas être confondu avec le facteur humidex canadien qui utilise une autre formule pour quantifier le même effet.
