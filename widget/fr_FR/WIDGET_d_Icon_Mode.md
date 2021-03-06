---
layout: default
lang: fr_FR
title: Widget "Icon_Mode"
description: explication Widget "Icon_Mode"
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une valeur <b>Info Texte</b>

<p><img src="../{{site.img}}/exemple/d/icone_mode.png" alt="Resultat" /></p>

# Info

## Merci

<blockquote>
    <ul>
        <li>Merci @Salviaf pour l'affichage de la durée</li>
        <li>Merci @Nicoraptor pour le code pour récupérer valeur Mode</li>
        <li>Merci @Antoinekl1 pour l'info et le code suite à la modif du plugin "Mode"</li>
    </ul>
</blockquote>

## A Savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

<hr />

## Valeur du mode

Pour que le widget fonctionne, il faut indiquer la valeur du mode dans les variables

<blockquote>
    <ul>
        <li><b>modex</b> : Valeur du mode</li>
        <li><b>x</b> : Remplacer <b>x</b> par le numéro de mode (valeur possible de 0 à 10)</li>
    </ul>
</blockquote>
Pour que le widget fonctionne dans le cas où les noms des commandes sont remplacés par des icônes, il faut indiquer le nom de l'icône dans les variables
<blockquote>
    <ul>
        <li><b>modex</b> : Nom de l'icône</li>
        <li><b>x</b> : Remplacer <b>x</b> par le numéro de mode (valeur possible de 0 à 10)</li>
    </ul>
</blockquote>

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels si le nom du mode ne correspond pas au nom de l'image :

<blockquote>
    <ul>
        <li><b>logox</b> : Permet de choisir l'image pour la valeur pour le mode <i>(valeur par défaut : <b>Nom_MODE</b>)</i></li>
        <li><b>logo_typex</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo</i> (par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
        <li><b>x</b> : Remplacer <b>x</b> par le numéro de mode (valeur possible de 0 à 10)</li>
        <li><b>Nom_MODE</b> : correspond au nom exact de l'image</li>
    </ul>
</blockquote>

## Sous dossier

Il possible d'ajouter les images dans des sous dossiers, (la variable est valable pour l'ensemble des valeurs)

<blockquote>
    <ul>
        <li><b>dossier</b> : Nom du dossier (Par défaut : Chauffage)</li>
        <li><a href="./list_img">Listes des images par dossiers</a></li>
    </ul>
</blockquote>

## Taille des images ou des icônes

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>Pourcentage</b> : Permet de choisir la taille en "px" ou "%" <i>(valeur par défaut : NO donc "px")</i></li>
        <ul>
            <li><i>Pourcentage = NO</i> la taille sera en "px"</li>
            <li><i>Pourcentage = YES</i> la taille sera en "%"</li>
        </ul>
        <li><b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 80)</i></li>
        <li><b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 80)</i></li>
    </ul>
</blockquote>

## Autres paramétrages possibles et Aide

<blockquote>
        <ul>
            <li><a href="{{site.baseurl}}/help/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
            <li><a href="{{site.baseurl}}/help/{{page.lang}}/config_info">Aide ajout des paramètres pour un widget Info</a></li>
            <li><a href="{{site.baseurl}}/help/{{page.lang}}/error">Paramètrage image de défaut</a></li>
            <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats">Afficher les statistiques</a></li>
            <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats_temps">Affichage des informations de durée sur les widgets info (binaire, numérique)</a></li>
            <li><a href="{{site.baseurl}}/help/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
        </ul>
</blockquote>

# Exemple Paramétrage d'un mode

<p><img src="./../{{site.img}}/JEEDOM_Icon_Mode_Para mode.png" alt="exemple Para" /></p>
<hr />

## Exemple 1

Un Premier exemple avec le mode0 = CONFORT et le nom de l'image est "CONFORT.PNG"

<blockquote>
        <ul>
            <li><b>mode0</b> : renseigner la valeur <b>CONFORT</b></li>
            <li><b>logo0</b> : Il n'est pas nécessaire de le renseigner vu que le nom du mode est identique au nom de l'image</li>
            <li><b>logo_type0</b> : Il n'est pas necessaire de le renseigner vu que l'extension de l'image est <i>png</i></li>
        </ul>
</blockquote>

## Exemple 2

Un deuxième exemple avec le mode5 = PURGE et le nom de l'image est "puitsvide.PNG"

<blockquote>
        <ul>
            <li><b>mode5</b> : renseigner la valeur <b>PURGE</b></li>
            <li><b>logo5</b> : renseigner la valeur <b>puitsvide</b></li>
            <li><b>logo_type5</b> : Il n'est pas nécessaire de le renseigner vu que l'extension de l'image est <i>png</i></li>
        </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Icon_Mode/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Icon_Mode/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Icon_Mode/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Icon_Mode/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
