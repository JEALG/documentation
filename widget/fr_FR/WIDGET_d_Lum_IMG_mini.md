---
layout: default
lang: fr_FR
title: Widget "Luminosité-IMG-Mini"
description: Widget Luminosité-IMG-Mini
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>

<p><img src="../{{site.img}}/exemple/d/lumi.png" alt="Resultat" /></p>

# A savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>logo_level1</b> : Permet de choisir l'image pour la valeur  pour le niveau 1 <i>(valeur par défaut : moon)</i></li>
        <li><b>logo_level1_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo_level1</i> (par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
        <li><b>logo_level2</b> : Permet de choisir l'image pour la valeur  pour le niveau 2 <i>(valeur par défaut : cloud)</i></li>
        <li><b>logo_level2_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo_level2</i> (par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
        <li><b>logo_level3</b> : Permet de choisir l'image pour la valeur  pour le niveau 3 <i>(valeur par défaut : sun)</i></li>
        <li><b>logo_level3_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo_level3</i> (par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
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
        <li><b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 65)</i></li>
        <li><b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 70)</i></li>
    </ul>
</blockquote>

## Paramétrage des Niveaux

Il est possible de modifier les niveaux

<blockquote>
    <ul>
        <li><b>level_1</b> : Niveau Bas (nuit) <i>(valeur par défaut : 20)</i></li>
        <li><b>level_2</b> : Niveau Haut (jour) <i>(valeur par défaut : 100.0)</i></li>
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
            <TD width="25%" rowspan="4">leg_pos</TD>
            <TD width="25%" align="center">low<br/>(valeur par défaut)</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/lumi.png" alt="Resultat - Bas" /></TD>
        </TR>
        <TR>
            <TD width="25%" align="center">right</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/lumi_r.png" alt="Resultat - Droite" /></TD>
        </TR>
        <TR>
            <TD width="25%" align="center">left</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/lumi_l.png" alt="Resultat - Gauche" /></TD>
        </TR>
        <TR>
            <TD width="25%" align="center">top</TD>
            <TD width="50%" align="center"><img src="../{{site.img}}/exemple/d/lumi_t.png" alt="Resultat - Gauche" /></TD>
        </TR>
    </TABLE>
</CENTER>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/config_info">Aide ajout des paramètres pour un widget Info</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/error">Paramétrage image de défaut</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Luminosite-IMG-Mini/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Luminosite-IMG-Mini/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/help/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/help/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Luminosite-IMG-Mini/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Luminosite-IMG-Mini/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
