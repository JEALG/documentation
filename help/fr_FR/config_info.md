---
layout: default
lang: fr_FR
title: Paramétrage des widgets de type info
description: explication Aide pour le paramétrage des widgets de type info (binaire, numAide pour le paramétrage des widgets de type info (binaire, numérique)
---

[back](./)

> **Une vidéo pour aider les nuls : <a href="https://www.youtube.com/watch?v=wiMh8rmfdKU">Virtuel pour les nuls</a>**

Ici l'exemple d'un équipement fait avec le plugin Virtuel, il faut paramétrer les infos suivantes :

<p><img src="../{{site.img}}/config_info_1.png" alt="Aide 1" width="700"/></p>

# Paramétrage de l'équipement

## La commande d'info

- <b>En marron</b> : Nom de la commande

- <b>En Rouge</b> : Sous types
  _ Type : info
  _ Sous-Type : Binaire

- <b>En vert</b> : Options

  - Afficher : Cocher cette case
  - Historiser : Permet d'historiser l'équipement (En option suivant les besoins)

- <b>En bleue</b> : Options
  - roue crantée permet de choisir le type de widget et les options

## Exemple de paramétrage

Voici l'exemple voulu

<p><img src="../{{site.img}}/multi_binaire.png" alt="Résultat" /></p>

## Les commandes d'action

voir l'exemple dans la doc <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/config_action">Aide pour le paramétrage des widgets de type action</a>

# Choix du widget

- Cliquer sur la roue crantée de la commande info
<p><img src="../{{site.img}}/config_roue.png" alt="Roue Crantée" width="100"/></p>

- Ensuite sélectionner l'onglet <b><i>Affichage</i></b> (flèche en violet)<br/>
<p><img src="../{{site.img}}/config_onglet_affichage_info.png" alt="Onglet Affichage" width="700" /></p><br/>

- Ensuite sélectionner le widget <b><i>Multiinfo-Binaire</i></b> (flèche en noir) pour la représentation <i>Dashboard</i> et <i>Mobile</i><br/>

# Ajout des paramètres

- Ajouter les variables ci-dessous en cliquant sur le bouton <b><i>Ajouter</i></b> (flèche en orange)<br/>
<p><img src="../{{site.img}}/config_onglet_affichage_info.png" alt="Onglet Affichage" width="700" /></p><br/>

<CENTER>
    <TABLE width="60%">
        <TR>
            <th scope="col" width="50%">Nom</th>
            <th scope="col" width="50%">Valeur</th>
        </TR>
        <TR>
            <TD width="50%">logoON</TD>
            <TD width="50%">al_type0_off</TD>
        </TR>
        <TR>
            <TD width="50%">logoOFF</TD>
            <TD width="50%">al_type0_on</TD>
        </TR>
        <TR>
            <TD width="50%">dossier</TD>
            <TD width="50%">alarme</TD>
        </TR>
    </TABLE>
</CENTER>

<hr />
[back](./)
