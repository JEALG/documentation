# Plugin Rosée - Givre - Tendance

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Troubleshotting

- Je n'ai pas d'informations qui remontent

> Il faut bien indiquer les équipements nécessaires pour les différents calculs.<br/>
> On peut rechercher les équipements grâce au bouton de recherche de l’équipement.

- Le point de givrage est égal 5°C

> La température dépasse 5°C donc le point de givrage n'est plus calculé et sa valeur est fixée à 5.

- Le calcul de la tendance ne se fait pas

> Il faut attendre 4h pour avoir des résultats corrects lors de la création de l'équipement.
> L'équipement doit avoir l'historique d'activé pour fonctionner et avoir "Répéter les valeurs identiques" sur Oui.

## Message d'erreur

### Le champs "Calcul" ne peut être vide

```
Le champ "Calcul" ne peut être vide
```

> Il faut vérifier que le champ calcul ne soit pas vide ou égal à aucune<br/>

![Calcul Vide](../{{site.img}}/erreur_calcul_vide.png)

### Le champ "Température" ne peut être vide

```
Le champ "Température" ne peut être vide
```

> Il faut vérifier qu'un équipement soit sélectionné dans le champ avec la flèche bleue (voir image ci-dessous)<br/>

### Le champ "Humidité Relative" ne peut être vide

```
Le champ "Humidité Relative" ne peut être vide
```

> Il faut vérifier qu'un équipement soit sélectionné dans le champ avec la flèche rouge (voir image ci-dessous)<br/>

### Le champ "Pression Atmosphérique" ne peut être vide

```
Le champ "Pression Atmosphérique" ne peut être vide
```

> Il faut vérifier qu'un équipement soit sélectionné dans le champ avec la flèche orange (voir image ci-dessous). Cette erreur apparait uniquement si le champ **Type de Calcul** a la valeur **_Tendance Météo_**<br/>

![Calcul Vide](../{{site.img}}/erreur_champ_vide.png)

### L'historique de la commande Pression doit être activé

```
L'historique de la commande xxx doit être activé
```

> l'historique de la commande xx doit ête obligatoirement activé.
(voir image ci-dessous)<br/>

![Historique](../{{site.img}}/pression1.png)
<br/>
![Historique](../{{site.img}}/pression2.png)

Dans certain cas, il est aussi conseillé d'activer "Répéter les valeurs identiques" pour éviter d'avoir l'erreur durant les calculs
![Historique](../{{site.img}}/pression3.png)
