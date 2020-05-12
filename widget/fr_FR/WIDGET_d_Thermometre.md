---
layout: default
lang: fr_FR
title: Widget "Temperature thermometre"
description: explication widget Temperature thermometre
---
[back](./)

Widget pour Jeedom permettant d'afficher une icône pour une fonction de type <b>Info Numérique</b>
<p><img src="../img/exemple/d/temperature.png" alt="Resultat" /></p>

# A savoir
<blockquote>
<b>Afin de simplifier la gestion des images, depuis le 10/09/2019, il est nécessaire d'avoir le </b><a href="WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>
</blockquote>

# Paramétrage
## Affichage de l'historique ou min max sur la gauche
<blockquote>
    <ul>
        <li><b>min_max</b> : Affiche par défaut le min et max configurer dans l'équipement <i>(valeur par défaut : X)</i></li>
        <p><img src="../img/JEEDOM_Thermometre_MIN_MAX.png" alt="INFO" /></p>
        <li><b>min_max</b> : utilise le maxi et le mini de l'historique, <i>la variable doit ête vide</i></li>
    </ul>
</blockquote>

## Taille du texte
<blockquote>
    <ul>
        Il est possible sur ce widget de modifier la taille du texte, cette fonction ne fonctionne qu'avec le Core V3
        <a href="{{site.baseurl}}/help/{{page.lang}}/size">Changer la Taille du texte de l'historique</a>
    </ul>
</blockquote>


## Autres paramétrages possible et Aide
<blockquote>
    <ul>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/">Aide (Ensemble de la documentation)</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/config_info">Aide ajout des paramétres pour un widget Info</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/error">Paramétrage image de défaut</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/stats">Afficher les statistiques</a></li>
        <li><a href="{{site.baseurl}}/help/{{page.lang}}/para">Ajouter les paramètres sur un widget</a></li>
    </ul>
</blockquote>


# Télécharger les sources
><a href="{{site.baseurl}}/help/{{page.lang}}/install_manu">Aide pour l'installation manuelle des widgets</a>
<br/>

<li><a href="https://github.com/JEALG/JEEDOM-Thermometre/tree/masterv4">Télécharger les sources du Widget pour le Core V4</a></li>
<li><a href="https://github.com/JEALG/JEEDOM-Thermometre/tree/master">Télécharger les sources du Widget pour le Core V3</a></li>

# Troubleshotting

- Je n'ai pas l'historique et l'option historique non visible dans la configuration de la commande sur les widgets de type info
<p><img src="{{site.baseurl}}/help/img/troubleshotting_1.png" alt="Troubleshotting Statistique" width="500" /></p>
>Il faut vérifier que l'option ***Afficher les statistiques sur les widgets*** est active
>* <a href="{{site.baseurl}}/help/{{page.lang}}/stats">Aide pour afficher les statistiques</a>

<hr />
# Changelog
<a href="https://github.com/JEALG/JEEDOM-Thermometre/commits/masterv4">Changelog WIDGET pour le Core V4</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Thermometre/commits/master">Changelog WIDGET pour le Core V3</a><br/>
<a href="https://github.com/JEALG/JEEDOM-Widget_JAG-doc/commits/master">Changelog DOC</a>

<hr />
[back](./)