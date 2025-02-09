# Plugin Temperature

<img src="{{site.baseurl}}/plugin-temperature/{{site.img}}/temperature_icon.png" class="pluginLogo" width="100" />

## Description

Ce plugin permet de calculer l'effet du vent sur la température ressentie, windchill (plutôt lorsque les températures sont basses), ainsi que l'effet d'inconfort provoqué par le taux d'humidité lorsque les températures sont élevées (humidex).

## Configuration

Le plugin ne comporte pas de configuration générale.
Il faut ajouter des équipements pour la température, l’humidité et la vitesse du vent
Il est possible d'indiquer :

- Un seuil d'alerte pour l'indice de chaleur (HUMIDEX). Par défaut, c'est 40°C qui déclenche l'alerte
- Un seuil de pré-alerte pour l'indice de chaleur (HUMIDEX). Par défaut, c'est 30°C qui déclenche la pré-alerte

## Températures ressenties

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
