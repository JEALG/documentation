---
layout: default
lang: fr_FR
title: Widget "VoyantMulticouleur
description: explication Bouton en forme de voyant Multi couleur
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>action</b>

<p><img src="../{{site.img}}/exemple/d/voyant_multicouleur.png" alt="Resultat" /></p>
<blockquote>
Les visu à utiliser sont :
</blockquote>

<p><img src="../{{site.img}}/visuel/voyant.png" alt="Visuels" /></p>

# A savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

## Choix de la couleur

Pour choisir la couleur, il faut ajouter les paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>CouleurON</b> : Permet de choisir la couleur du voyant pour la valeur ON <i>(valeur par défaut : GN)</i></li>
        <li><b>CouleurOFF</b> : Permet de choisir la couleur du voyant pour la valeur OFF <i>(valeur par défaut : RD)</i></li>
        <li><b>Les valeurs possibles </b> : BK, BU, GN, OR, RD, WH, YE</li>
    </ul>
</blockquote>

## Choix de la forme

Pour choisir la forme, il faut ajouter les paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>FormeON</b> : Permet de choisir la forme du voyant pour la valeur ON <i>(valeur par défaut : ROND)</i></li>
        <li><b>FormeOFF</b> : Permet de choisir la forme du voyant pour la valeur OFF <i>(valeur par défaut : ROND)</i></li>
        <li><b>Les valeurs possibles</b> : ROND, CARRE</li>
    </ul>
</blockquote>

## Choix de l'extension

Pour choisir le type d'extension de l'image

<blockquote>
    <ul>
        <li><b>logoON_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoON</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i></li>
        <li><b>logoOFF_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoON</i> (par exemple: 'gif', 'jpg', etc.....)<i> (valeur par défaut : png)</i></li>
    </ul>
</blockquote>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/config_info">Aide ajout des paramètres pour un widget Info</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

### Ajout d'image

Il est possible d'inclure d'autres icônes dans le widget.<br/>
Le nommage des images est normalisé et doit respecter le format suivant :

<blockquote>
    <ul>
        <li><b>Image pour la valeur pour le niveau</b> : FORME_COULEUR</li>
        <li><i>Remplacer <b>FORME</b> par la valeur rond ou carre ou Autres</i></li>
        <li><i>Remplacer <b>COULEUR</b> par la valeur bk, bu, gn, or, rd, wh, ye</i></li>
    </ul>
    <ul>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-VoyantMulticouleur/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-VoyantMulticouleur/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-VoyantMulticouleur/commits/masterv4">Changelog WIDGET Pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-VoyantMulticouleur/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
