---
layout: default
title: Plugin Rosee - documentation
lang: fr_FR
pluginId: rosee
---

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

# Description

Ce plugin permet d'obtenir le point de rosée pour savoir si l'herbe sera mouillée le matin, ou bien en hiver savoir s'il va falloir gratter le pare-brise.
Pour fonctionner, on doit indiquer un équipement température et un équipement humidité (extérieures, bien-sûr…).
Il est aussi possible de calculer la tendance Météo à venir en se basant de l'évolution de la météo.

# Configuration

Le plugin ne comporte pas de configuration générale, il faut :

> Choisir une méthode de calcul :

    - Humidité absolue
    - Point de Givre
    - Point de Rosée
    - Point de Rosée et Point de Givre
    - Tendance Météo

> Renseigner les champs obligatoires suivant la méthode de calcul :

    - Équipement "Température" (°C)
    - Équipement "Humidité Relative" (%)
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

> - Rosee/Tendance (Icône 40x40) (Widget par défaut)

<p><img src="../{{site.img}}/visu_tendance.png" width="150" alt="Visu Tendance 40x40" /></p>

> - Rosee/Tendance 80x80 (Icône 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="150" alt="Visu Tendance 80x80" /></p>
