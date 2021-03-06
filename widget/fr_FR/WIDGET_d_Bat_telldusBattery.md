---
layout: default
lang: fr_FR
title: Widget " Batterie-telldusBattery"
description: explication widget Batterie-telldusBattery
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique </b>

<p><img src="../{{site.img}}/exemple/d/bat_telldusbatter.png" alt="Resultat" /></p>

# A savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>logo</b> : Permet de choisir l'image pour la valeur<i>(valeur par défaut : battery_)</i></li>
        <li><b>logo_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoON</i>(par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
    </ul>
</blockquote>

## Taille de l'image

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 65)</i></li>
        <li><b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 30)</i></li>
    </ul>
</blockquote>

## Paramétrage des Niveaux

Il est possible de personnaliser les niveaux :

<blockquote>
    <ul>
        <li><b>level_0</b>   : Niveau 0 <i>(valeur par défaut : 0)</i></li>
        <li><b>level_20</b>  : Niveau 20 <i>(valeur par défaut : 20)</i></li>
        <li><b>level_40</b>  : Niveau 40 <i>(valeur par défaut : 40)</i></li>
        <li><b>level_60</b>  : Niveau 60 <i>(valeur par défaut : 60)</i></li>
        <li><b>level_80</b>  : Niveau 80 <i>(valeur par défaut : 80)</i></li>
        <li><b>level_100</b> : Niveau 100 <i>(valeur par défaut : 100)</i></li>
    </ul>
</blockquote>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/config_info">Aide ajout des paramètres pour un widget Info</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/error">Paramétrage image de défaut</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats_temps">Affichage des informations de durée sur les widgets info (binaire, numérique)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

### Ajout d'image

Il est possible d'inclure d'autres icônes dans le widget.<br/>
Le nommage des images est normalisé et doit respecter le format suivant :

<blockquote>
    <ul>
        <li><b>Image pour la valeur pour le niveau</b> : battery_Niveau</li>
        <li><i>Remplacer <b>Niveau</b> par la valeur 0 ou 20 ou 40 ou 60 ou 80 ou 100</i></li>
    </ul>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Batterie-telldusBattery/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Batterie-telldusBattery/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Batterie-telldusBattery/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Batterie-telldusBattery/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
