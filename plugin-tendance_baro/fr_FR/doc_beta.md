# Plugin Tendance Baro

<img src="{{site.baseurl}}/plugin-tendance_baro/{{site.img}}/baro_icon.png" class="pluginLogo" width="100" />

## Description

Ce plugin permet de calculer la tendance météo à venir en se basant sur les évolutions de la pression atmosphérique des dernières heures

## Configuration

Le plugin ne comporte pas de configuration générale.
Il faut ajouter un équipement pour la pression atmosphérique.

> Cet équipement doit avoir l'historique activé

## Tendance Météo

> Sources :
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

Le plugin calcule 6 niveaux d'information

|  Niveau  | Tendance                           |                          Image du widget                           |
| :------: | :--------------------------------- | :----------------------------------------------------------------: |
| <b>0</b> | Forte dégradation, instable        | <img src="../images/tendance_0.png" alt="Tendance 0" width="40" /> |
| <b>1</b> | Dégradation, mauvais temps durable | <img src="../images/tendance_1.png" alt="Tendance 1" width="40" /> |
| <b>2</b> | Lente dégradation, temps stable    | <img src="../images/tendance_2.png" alt="Tendance 2" width="40" /> |
| <b>3</b> | Lente amélioration, temps stable   | <img src="../images/tendance_3.png" alt="Tendance 3" width="40" /> |
| <b>4</b> | Amélioration, beau temps durable   | <img src="../images/tendance_4.png" alt="Tendance 4" width="40" /> |
| <b>5</b> | Forte embellie, instable           | <img src="../images/tendance_5.png" alt="Tendance 5" width="40" /> |

## Le plugin met à disposition deux widgets pour la tendance :

> - Baro/Tendance (Icône 40x40) (Widget par défaut)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Baro/Tendance 80x80 (Icône 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>