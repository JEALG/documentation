---
layout: default
lang: fr_FR
title: Paramétrage image défaut Widget
description: Paramétrage image défaut Widget
---

[back](./)

En cas de défaut de valeur sur un widget de type info (binaire - Numérique), le widget affichage un icône d'erreur, il est possible de paramétrer celui-ci

# Paramétrage pour le "Dashboard"

En cas de défaut de valeur sur un widget de type info (binaire - Numérique), le widget affichage un icône d'erreur, il est possible de paramétrer celui-ci

<blockquote>
    <ul>
        <li><b>logoER</b> : Permet de choisir l'image pour la valeur ETAT en cas de problème <i>(valeur par défaut en général : oups)</i></li>
        <li><b>logoER_type</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoER</i>(par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
    </ul>
</blockquote>

# Paramétrage pour le "Mobile"

En cas de défaut de valeur sur un widget de type info (binaire - Numérique), le widget affichage un icône d'erreur, il est possible de paramétrer celui-ci

<blockquote>
    <ul>
        <li><b>logoER-M</b> : Permet de choisir l'image pour la valeur ETAT en cas de problème <i>(valeur par défaut en général : er_oups1)</i></li>
        <li><b>logoER_type-M</b> : Permet de choisir <i>l'extension</i> pour l'icône/image <i>logoER-M</i>(par exemple: 'gif', 'jpg', etc.....)<i>(valeur par défaut : png)</i></li>
    </ul>
</blockquote>

# Liste des images possibles

<p><img src="{{site.baseurl}}/{{site.widget}}/{{site.img}}/visuel/error.png" alt="Error" /></p>

# Cas Particulier

Pour les widgets suivants, il est possible d'indiquer le dossier de l'image d'erreur

<ul>
    <li><a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_d_Icon_Mode">Widget Dashboard : <b>Icon_Mode</b></a></li>
    <li><a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_m_Icon_Mode">Widget Mobile : <b>Icon_Mode (mobile)</b></a></li>
    <li><a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_d_Multi_info_Binaire">Widget Dashboard : <b>Multi info - Binaire</b></a></li>
    <li><a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_m_Multi_info_Binaire">Widget Mobile : <b>Multi info - Binaire (mobile)</b></a></li>
</ul>
<blockquote>
    <ul>
        <li><b>dossierER</b> : Permet de choisir le dossier pour l'image "Erreur" pour la version dashboard <i>(valeur par défaut : error)</i></li>
        <li><b>dossierER-M</b> : Permet de choisir le dossier pour l'image "Erreur" pour la version dashboard <i>(valeur par défaut : error)</i></li>
    </ul>
</blockquote>

# Cas Particulier pour les widgets Multi_info-Binaire

<ul>
    <li><a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_d_Multi_info_Binaire">Widget Dashboard : <b>Multi info - Binaire</b></a></li>
    <li><a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_m_Multi_info_Binaire">Widget Mobile : <b>Multi info - Binaire (mobile)</b></a></li>
</ul>

Petit rappel : la variable ci-dessous permet de récupérer ou pas les même infos que le Dashboard

<blockquote>
    <ul>
        <li><b>Dashboard-M</b> = <i>YES (valeur par défaut)</i> : Image identique au Dashboard</li>
        <li><b>Dashboard-M</b> = <i>NO</i>  : Image différente au Dashboard</li>
    </ul>
</blockquote>

Paramétrage image Erreur : Il est possible d'appliquer la même image que pour la valeur ON ou OFF

<blockquote>
    <ul>
        <li><b>para_ER</b> = <i>logoON</i> : l'image d'erreur sera identique que pour la valeur ON</li>
        <li><b>para_ER-M</b> = <i>logoON</i> : l'image d'erreur sera identique que pour la valeur ON</li>
        <li><b>para_ER</b> = <i>logoOFF</i> : l'image d'erreur sera identique que pour la valeur OFF</li>
        <li><b>para_ER-M</b> = <i>logoOFF</i> : l'image d'erreur sera identique que pour la valeur OFF</li>
        <li><b>para_ER</b> = <i> </i> (valeur vide) : l'image d'erreur sera identique que pour la valeur logoER <i>(valeur par défaut)</i></li>
        <li><b>para_ER-M</b> = <i></i> (valeur vide) : l'image d'erreur sera identique que pour la valeur logoER <i>(valeur par défaut)</i></li>
    </ul>
</blockquote>

 <hr />
[back](./)
