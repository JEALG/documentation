---
layout: default
lang: fr_FR
title: Widget "Biroute - vent"
description: explication widget Biroute - vent
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>

<p><img src="../{{site.img}}/exemple/d/biroute.png" alt="Resultat" /></p>

<p><img src="../{{site.img}}/visuel/vent.png" alt="Visuels" /></p>

<blockquote>
    <ul>
        <li>Toutes les images présentent dans le dossier <i><b>vent</b></i> ne sont utilisables avec ce widget, il faut que les images soient du style : </li>
        <li><b>Image</b> : image_xx => <b>xx</b> doit être égal à 0 ou 45 ou 90 ou over</li>
    </ul>
</blockquote>

# A savoir

> - <b>Pour le core V3 </b> : Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>

> - <b>Pour le core V4</b> :
>   - Il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le <a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>

# Paramétrage

## Choix de l'icône

Pour choisir le type de visuel à afficher, il faut ajouter les paramètres optionnels suivants :
Il n'est pas nécessaire de mettre ses paramètres si vous utilisez le paramétrage par défaut

<blockquote>
    <ul>
        <li><b>logo</b> : Permet de choisir l'image pour la valeur<i>(valeur par défaut : ve_manche2)</i></li>
        <li><b>logo_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logo</i>(par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
    </ul>
</blockquote>

<b>Attention</b>

<blockquote>
    <ul>
        <li>L'image change en fonction de la vitesse du vent, il ne faut pas mettre _xx dans le paramètre logo</li>
        <li>Si vous utilisez l'image par défaut, il n'est pas nécessaire d'ajouter le paramètre <b>logo</b></li>
        <li>Le Widget est basé sur la vitesse du vent en km/h, il faut donc convertir la vitesse du vent de m/s en km/h. Cela se fait directement depuis l'équipement, Il faut ajouter dans la configuration de l'équipement puis l'onglet configuration la valeur <b>#value#*3.6</b> dans le champ <i>Formule de calcul (#value# pour la valeur)</i>. Ne pas oublier ensuite de changer l'unité de la vitesse de vent</li>
    </ul>
</blockquote>

<p><img src="../{{site.img}}/exemple/d/biroute_1.png" alt="Resultat" /></p>

## Taille des images ou des icônes

Il est possible de spécifier la hauteur et la largeur des icônes ou images par l'ajout des paramètres optionnels suivants :

<blockquote>
    <ul>
        <li><b>sizeh</b> : Permet de choisir la hauteur de l'image <i>(valeur par défaut : 80)</i></li>
        <li><b>sizew</b> : Permet de choisir la largeur de l'image <i>(valeur par défaut : 80)</i></li>
    </ul>
</blockquote>

## Ajout d'image

Il est possible d'inclure d'autres icônes dans le widget.<br/>
Le nommage des images est normalisé et doit respecter le format suivant :

<blockquote>
    <ul>
        <li><b>Image</b> : type_xx</li>
        <li><i>Remplacer <b>type</b> par le nom de l'image</i></li>
        <li><i>Remplacer <b>xx</b> par la vitesse de vent (Valeur possible : 0, 45, 90, over)</i></li>
    </ul>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/add_img">Ajouter des images dans un widget</a></li>
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

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Biroute_vent/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Biroute_vent/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/help/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/help/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />

# Changelog

<a href="https://github.com/JEALG/JEEDOM-Biroute_vent/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Biroute_vent/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
