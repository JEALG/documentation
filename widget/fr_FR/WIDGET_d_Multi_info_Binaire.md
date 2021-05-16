---
layout: default
lang: fr_FR
title: Widget "Multi-info-Binaire"
description: Explication widget Multi-info-Binaire
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Binaire</b>

<p><img src="../{{site.img}}/exemple/d/multi_binaire.png" alt="Resultat" /></p>

# A savoir

<blockquote>
<b>Pour le Core V3, Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>
<b>Pour le Core V4, il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le </b><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>
</blockquote>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivants :

**Dans le cas de l'utilisation avec le nom de l'image normalisé**

> - <b>logo</b> : Permet de choisir l'image pour la valeur ON ou OFF <i>(pas de valeur par défaut)</i>
>   - <b>Attention avec cette variable</b>, il ne faut mettre **_\_off_** ou **_\_on_** à la fin du nom de l'image
>   - <b>l'utilisation de cette méthode désactive les variables <i>logoON</i> et <i>logoOFF</i></b>

> - <b>logo_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo</i> (par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)
> - Le nommage des images normalisées doit respecter le format suivant :
>   - <b>Image pour la valeur ON</b> : type_on
>   - <b>Image pour la valeur OFF</b> : type_off
>   - <i>Remplacer <b>type</b> par le nom de l'image</i>

**Dans le cas de l'utilisation avec le nom de l'image non normalisé**

> - <b>Logo pour la commande ON</b>
>   - <b>logoON</b> : Permet de choisir l'image pour la valeur ON <i>(valeur par défaut : fi_wh_off")</i>
>   - <b>logoON_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoON</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i>

> - <b>Logo pour la commande OFF</b>
>   - <b>logoOFF</b> : Permet de choisir l'image pour la valeur OFF <i>(valeur par défaut : fi_bu_on)</i>
>   - <b>logoOFF_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoOFF</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i>

## Sous dossier

Il possible d'ajouter les images dans des sous dossiers, (la variable est valable pour l'ensemble des valeurs)

> - <b>dossier</b> : Nom du dossier de l'image (Par défaut : divers)</li>
> - <a href="list_img">Listes des images par dossiers</a></li>

## Taille des images ou des icônes

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivants :

> - <b>Pourcentage</b> : Permet de choisir la taille en "px" ou "%" <i>(valeur par défaut : NO donc "px")</i>
>   - <i>Pourcentage = NO</i> la taille sera en "px"
>   - <i>Pourcentage = YES</i> la taille sera en "%"

> - <b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 80)</i>
> - <b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 80)</i>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/config_info">Aide pour le paramétrage des widgets de type infos</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats_temps">Affichage des informations de durée sur les widgets info (binaire, numérique, actions)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/para.html">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

## Exemple de paramétrage

> - <a href="{{site.baseurl}}/help/{{page.lang}}/config_info">Aide pour le paramétrage des widgets de type info (binaire, numérique, actions)</a>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Multi_info-Binaire/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_info-Binaire/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/help/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/help/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />
# Changelog
<a href="https://github.com/JEALG/JEEDOM-Multi_info-Binaire/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Multi_info-Binaire/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
