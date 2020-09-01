---
layout: default
lang: fr_FR
title: Widget "Multi-action"
description: Explication widget Multi-action
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Action ON/OFF</b>

<blockquote>
    Ce widget regroupe l'ensemble des différentes images de mes widgets
</blockquote>

<p><img src="../{{site.img}}/exemple/d/multi_action.png" alt="Resultat" /></p>

> Le widget inclus plusieurs icônes dans des sous dossiers
> <b>Ce widget remplace ces widgets : </b><a href="{{site.baseurl}}/{{site.archive}}/{{page.lang}}/WIDGET_d_Multi_action_Defaut">Archive widget Multi-action</a>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivant :

**Dans le cas de l'utilisation avec le nom de l'image normalisé**

> - <b>logo</b> : Permet de choisir l'image pour la valeur ON ou OFF <i>(pas de valeur par défaut)</i>

    * <b>Attention avec cette variable</b>, il ne faut mettre ***_off*** ou ***_on*** à la fin du nom de l'image
    *  <b>l'utilisation de cette méthode désactive les variables <i>logoON</i> et <i>logoOFF</i></b>

> - <b>logo_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo</i> (par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)
> - Le nommage des images normalisées doit respecter le format suivant :

    * <b>Image pour la valeur ON</b> : type_on
    * <b>Image pour la valeur OFF</b> : type_off
    * <i>Remplacer <b>type</b> par le nom de l'image</i>

**Dans le cas de l'utilisation avec le nom de l'image non normalisé**

> - <b>Logo pour la commande ON</b>

    * <b>logoON</b> : Permet de choisir l'image pour la valeur ON <i>(valeur par défaut : fi_wh_off")</i>
    * <b>logoON_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoON</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i>

> - <b>Logo pour la commande OFF</b>

    * <b>logoOFF</b> : Permet de choisir l'image pour la valeur OFF <i>(valeur par défaut : fi_bu_on)</i>
    * <b>logoOFF_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoOFF</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i>

## Sous dossier

Il possible d'ajouter de mettre les images dans des sous dossiers, (la variable est valable pour l'ensemble des valeurs)

<blockquote>
    <ul>
        <li><b>dossier</b> : Nom du dossier de l'image (Par défaut : divers)</li>
        <li><a href="list_img">Listes des images par dossiers</a></li>
    </ul>
</blockquote>

## Taille des images ou des icônes

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivant :

> - <b>Pourcentage</b> : Permet de choisir la taille en "px" ou "%" <i>(valeur par défaut : NO donc "px")</i>

    * <i>Pourcentage = NO</i> la taille sera en "px"
    * <i>Pourcentage = YES</i> la taille sera en "%"

> - <b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 80)</i>
> - <b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 80)</i>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/config_action">Aide pour le paramétrage des widgets de type action</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats_temps">Affichage des informations de durée sur les widgets info (binaire, numérique, actions)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

## Exemple de paramétrage

> - <a href="{{site.baseurl}}/help/{{page.lang}}/config_action">Aide pour le paramétrage des widgets de type action</a>

### Ajout d'image

Il est possible d'inclure d'autres icônes dans le widget.<br/>
Le nommage des images n'est pas normalisé sur ce widget\$

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/help/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>
> <br/>

<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>

<hr />
# Changelog
<a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
