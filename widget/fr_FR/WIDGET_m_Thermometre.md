---
layout: default
lang: fr_FR
title: Widget "Temperature thermometre (mobile)"
description: explication widget Temperature thermometre (mobile)
---

[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>

<p><img src="../{{site.img}}/exemple/m/temperature.png" alt="Resultat" /></p>

# A savoir

<blockquote>
<b>Pour le Core V3, Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>
<b>Pour le Core V4, il faut copier le contenu dans du dossier <i>img</i> qui se trouve dans le </b><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Ensemble des Images pour Core V4</a> dans le dossier : <b><i>html/data/img</i></b>
</blockquote>

# Paramétrage

## Affichage de l'historique ou min max sur la gauche

<blockquote>
    <ul>
        <li><b>min_max-M</b> : Affiche par défaut le min et max configurés dans l'équipement <i>(valeur par défaut : X)</i></li>
        <p><img src="../{{site.img}}/JEEDOM_Thermometre_MIN_MAX.png" alt="INFO" /></p>
        <li><b>min_max-M</b> : Utilise le maxi et le mini de l'historique, <i>la variable doit être vide</i></li>
    </ul>
</blockquote>

## Autres paramétrages possibles et Aide

<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/config_info">Aide ajout des paramètres pour un widget Info</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/error">Paramétrage image de défaut</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>

# Télécharger les sources

> <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>

<li><a href="https://github.com/JEALG/JEEDOM-Thermometre--mobile/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Thermometre--mobile/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut/tree/images">Télécharger les images pour le Core V4</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/{{site.help}}/{{site.img}}/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/{{site.help}}/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />
# Changelog
<a href="https://github.com/JEALG/JEEDOM-Thermometre--mobile/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Thermometre--mobile/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)
