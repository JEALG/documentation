---
layout: default
lang: fr_FR
title: Widget "Store-banne"
description: explication Store-banne
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>

<p><img src="../{{site.img}}/exemple/d/store_banne.png" alt="Resultat" /></p>

# A savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>logo</b> : Permet de choisir l'image pour la valeur <i>(valeur par défaut : st_banne_pos)</i></li>
        <li><b>logo_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i></li>
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

## Masquer la valeur

Il est possible de masquer la valeur de l'ouverture :

<blockquote>
    <ul>
        <li><b>masque_valeur</b> : Permet de masquer la valeur <i>(valeur par défaut :NO)</i></li>
        <li>variable avec la valeur <b>NO</b> ne masque pas la valeur <i>(valeur par défaut)</i></li>
        <li>variable avec la valeur <b>YES</b> masque la valeur</li>
    </ul>
</blockquote>

## Inversion sens image

Si l'équipement a la valeur 0 pour l'ouverture, il est possible d'inverser le sens

<blockquote>
    <ul>
        <li><b>levelINV = 0</b> Ouverture = 100% <i>(valeur par défaut : 0)</i></li>
        <li><b>levelINV = 1</b> Ouverture = 0%  <i></i></li>
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
        <li><b>Image</b> : typex</li>
        <li><i>Remplacer <b>type</b> par le nom de l'image</i></li>
        <li><i>Remplacer <b>x</b> par le niveau (Valeur possible : 0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100)</i></li>
    </ul>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Store-banne/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Store-banne/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/help/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/help/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Store-banne/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Store-banne/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
