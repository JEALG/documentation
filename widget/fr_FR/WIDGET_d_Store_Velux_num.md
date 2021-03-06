---
layout: default
lang: fr_FR
title: Widget "Store-VELUX (numérique)"
description: explication widget Store-VELUX (numérique)
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>

<p><img src="../{{site.img}}/exemple/d/store_velux.png" alt="Resultat" /></p>

# A savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>logo</b> : Permet de choisir l'imag e<i>(valeur par défaut : st_volet_pos)</i></li>
        <li><b>logo_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i></li>
    </ul>
</blockquote>

## Taille des images ou des icônes

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 90)</i></li>
        <li><b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 90)</i></li>
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

## Paramétrage des Niveaux

Il est possible de personnaliser les niveaux :

<blockquote>
    <ul>
        <li><b>level_0</b> : Niveau 0 <i>(valeur par défaut : 0) </i></li>
        <li><b>level_1</b> : Niveau 1 <i>(valeur par défaut : 17)</i></li>
        <li><b>level_2</b> : Niveau 2 <i>(valeur par défaut : 35)</i></li>
        <li><b>level_3</b> : Niveau 3 <i>(valeur par défaut : 45)</i></li>
        <li><b>level_4</b> : Niveau 4 <i>(valeur par défaut : 55)</i></li>
        <li><b>level_5</b> : Niveau 5 <i>(valeur par défaut : 63)</i></li>
        <li><b>level_6</b> : Niveau 6 <i>(valeur par défaut : 73)</i></li>
        <li><b>level_7</b> : Niveau 7 <i>(valeur par défaut : 84)</i></li>
        <li><b>level_8</b> : Niveau 8 <i>(valeur par défaut : 92)</i></li>
        <li><b>level_9</b> : Niveau 9 <i>(valeur par défaut : 95)</i></li>
        <li><b>level_10</b> : Niveau 10 <i>(valeur par défaut : 100)</i></li>
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
        <li><b>Image</b> : type-x</li>
        <li><i>Remplacer <b>type</b> par le nom de l'image</i></li>
        <li><i>Remplacer <b>x</b> par le niveau (Valeur possible : 0, 1, 10, 20, 30, 40, 50, 60, 70, 80, 99)</i></li>
    </ul>
</blockquote>
<blockquote>
Les images en fonction des niveaux
    <ul>
        <li><b>Niveau = level_0</b> : Store-0</li>
        <li><b>Niveau > level_0 et Niveau ≤ Level_1</b> : Store-1</li>
        <li><b>Niveau > level_1 et Niveau ≤ Level_2</b> : Store-10</li>
        <li><b>Niveau > level_2 et Niveau ≤ Level_3</b> : Store-20</li>
        <li><b>Niveau > level_3 et Niveau ≤ Level_4</b> : Store-30</li>
        <li><b>Niveau > level_4 et Niveau ≤ Level_5</b> : Store-40</li>
        <li><b>Niveau > level_5 et Niveau ≤ Level_6</b> : Store-50</li>
        <li><b>Niveau > level_6 et Niveau ≤ Level_7</b> : Store-60</li>
        <li><b>Niveau > level_7 et Niveau ≤ Level_8</b> : Store-70</li>
        <li><b>Niveau > level_8 et Niveau ≤ Level_9</b> : Store-80</li>
        <li><b>Niveau > level_9 et Niveau ≤ Level_10</b> : Store-99</li>
    </ul>
</blockquote>
<blockquote>
    <li><a href="{{site.baseurl}}/help/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Store-Velux-num/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Store-Velux-num/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/help/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/help/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Store-Velux-num/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Store-Velux-num/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
