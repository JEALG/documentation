---
layout: default
lang: fr_FR
title: Widget "Baromètre"
description: explication widget Baromètre
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>

<p><img src="../{{site.img}}/exemple/d/baro.png" alt="Resultat" /></p>

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

## Taille des images ou des icônes

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 80)</i></li>
        <li><b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 83)</i></li>
    </ul>
</blockquote>

## Position Légende

Il est possible de déplacer la légende

<CENTER>
    <TABLE width="100%">
        <TR>
            <th scope="col" width="25%">Nom de la variable</th>
            <th scope="col" width="25%">valeur</th>
            <th scope="col" width="37%">Valeur</th>
        </TR>
        <TR>
            <TD width="25%" rowspan="3">leg_pos</TD>
            <TD width="25%" align="center">right<br/>(valeur par défaut)</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/baro.png" alt="Resultat - Droite" /></TD>
        </TR>
        <TR>
            <TD width="25%" align="center">left</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/baro_le.png" alt="Resultat - Gauche" /></TD>
        </TR>
        <TR>
            <TD width="25%" align="center">bottom</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/baro_l.png" alt="Resultat - Bas" /></TD>
        </TR>
    </TABLE>
</CENTER>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/config_info">Aide ajout des paramètres pour un widget Info</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/error">Paramétrage image de défaut</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/stats_temps">Affichage des informations de durée sur les widgets info (binaire, numérique)</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

### Ajout d'image

Il est possible d'inclure d'autres icônes dans le widget.<br/>
Le nommage des images est normalisé et doit respecter le format suivant :

<blockquote>
    <ul>
        <li><b>Image</b> : type_x</li>
        <li><i>Remplacer <b>type</b> par le nom de l'image</i></li>
        <li><i>Remplacer <b>x</b> par le niveau (Valeur possible : 940, 950, 960, 970, 980, 990, 1000, 1010, 1020, 1030, 1040, 1050, 1060)</i></li>
    </ul>
    <ul>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Barometre/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Barometre/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/{{site.help}}/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Barometre/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Barometre/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
