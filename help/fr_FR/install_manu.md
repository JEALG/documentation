---
layout: default
lang: fr_FR
title: Installation Manuelle des widgets
description: Installation Manuelle des widgets pour le Core V4
---

[back](./)

# Info

> Comme vous le savez le market widget disparu. Si vous voulez continuer à utiliser mes widgets et avoir les mises à jour.
> Voici une méthode vous permettant d'installer et de faire les mises à jour.

# A Savoir

<blockquote>
    Pour l'ensemble de mes widgets, il est nécessaire d'avoir le widget <a href="{{site.baseurl}}/{{site.widget}}/{{page.lang}}/WIDGET_d_Multi_action_Defaut">Widget Dashboard : <b>Multi-action</b></a>
<br/>
</blockquote>

# Récupérer les sources

Les sources sont disponibles sur mon Github
<a href="https://github.com/JEALG"> JAG Github</a><br/>
Choisir le widget voulu
<br/>
voici un exemple pour récupérer les sources
<a href="https://github.com/JEALG/JEEDOM-Multi_action-Defaut">JEEDOM-Multi_action-Defaut</a>

<p><img src="../{{site.img}}/Github_branche_1.png" alt="Choix Branche" width="500"/></p>
Sélectionner la branche voulue :
<blockquote>
    <ul>
        <li>Beta : Version en test</li>
        <li>Master : Version Stable pour le Core <b>V3</b></li>
        <li>MasterV4 : Version Stable pour le Core <b>V4</b></li>
    </ul>
</blockquote>
Cliquer sur <i>Clone or download</i> ensuite cliquer sur <i>Download ZIP</i>
<p><img src="../{{site.img}}/Github_branche_2.png" alt="Download" width="500"/></p>

# Plugin nécessaire "jeeXplorer"

Il faut installer le plugin JeeXplorer

> Attention : Comme tout explorateur de fichiers, celui-ci vous permet d'accéder et d'éditer tous les fichiers présents dans le répertoire racine de Jeedom.

> Attention donc aux mauvaises manipulations qui pourraient rendre votre Jeedom complètement inopérant !

<ul>
    <li><a href="https://www.jeedom.com/market/index.php?v=d&p=market&type=plugin&categorie=programming&&name=JeeXplorer">Lien Market vers le plugin</a></li>
    <li><a href="https://kiboost.github.io/jeedom_docs/plugins/jeexplorer/fr_FR/">Lien vers la doc du plugin</a></li>
</ul>

# Installation ou Mise à jour

Dézipper le fichier téléchargé du widget voulu
<br/>
Se rendre dans Jeedom et ouvrir le plugin <i>Organisation/jeeXplorer</i>
<br/>
Se rendre dans le dossier correspondant au type de widget

<b>L'ensemble des fichiers sont à copier dans les dossiers suivants Pour le Core V4 :</b>

> - Pour les widgets du dashboard : <i><b>html/data/customTemplates/dashboard/</b></i>
> - Pour les fichiers images se trouvant dans le widget Multi-action <b>img</b>, copier le contenu dans le dossier : <i><b>html/data/img/</b></i>
> - Pour les widgets du mobile : html/data/customTemplates/mobile/ <i>Le nom des "repository" de mes widgets mobiles se termine par "--mobile"</i>

<ul>
  <b>L'ensemble des fichiers sont à copier dans les dossiers suivants Pour le Core V3 :</b>
    <blockquote>
        <ul>
            <li>html/plugins/{{site.widget}}/core/template/dashboard/</li>
            <li>html/plugins/{{site.widget}}/core/template/mobile/ <i>Le nom des "repository" de mes widgets mobiles se termine par "--mobile"</i></li>
        </ul>
    </blockquote>
</ul>

<p><img src="../{{site.img}}/add_widget_1.png" alt="ADD" width="500" /></p>
Cliquer sur Envoyer les fichiers
<p><img src="../{{site.img}}/add_widget_2.png" alt="ADD" width="500" /></p>
Cliquer ensuite sur <i>Sélectionner les fichiers à envoyer</i> ou pour envoyer l'ensemble des dossiers, cliquer sur <i>Choisir le dossier</i>
<p><img src="../{{site.img}}/add_widget_3.png" alt="ADD" width="200" /></p>

<hr />
[back](./)
