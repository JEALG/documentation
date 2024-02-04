---
layout: default
title: Plugin Rosee - Changelog
lang: fr_FR
pluginId: rosee
---

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Important

> **_Pour rappel_** s'il n'y a pas d'information sur la mise à jour, c'est que celle-ci concerne uniquement de la mise à jour de documentation, de traduction ou de corrections de bugs mineurs.

## Changelog

### 2024

### 04/02/2024

- Suppression lien community suite changement core 4.4
- Amélioration affichage sous tableau

### 14/01/2024

- Amélioration pour core V4.4

### 2023

#### 08/10/2023

- Amélioration info vers Community pour le Core 4.4
- Typo

#### 02/06/2023

- Mise à jour info market

#### 02/04/2023

- Correction pour core 4.4
- Version mini Core pour le plugin est 4.2

#### 20230327

- Typo

### 2022

#### Version 20220212

- Affichage Core v4.2
- Fonction Core v4.3
- La méthode js jeedom.eqLogic.builSelectCmd a été renommée correctement : jeedom.eqLogic.buildSelectCmd.

### 2021

#### Version 20211101

- Ajout Info Json
- Ajout info pression et correction création des commandes
- Correction création des commandes tendance

#### Version 20211023

- Mise à jour suite au changement du core v4.2

#### Version 20210728

- Amélioration pour Core v4.2

#### Version 20210510

- Ajout info dans log

#### Version 20210226

- Correction température ressentie

#### Version 20210213

- Affichage tableau Core v4.2 (beta)
- Correction Objet Parent
- Amélioration générale de l'affichage

### 2020

#### Version 20201208

- Correction Bug Calcul Humidex
- Correction Bug divers

#### Version 20201207

- Correction Bug création des commandes
- Correction Bug Min et Max des commandes numériques
- Ajout calcul température ressentie pour l'hiver https://community.jeedom.com/t/temperature-ressentie/44377/2?u=jag

#### Version 20201129

- Amélioration de l'affichage, ajout info bulle sur les commandes
- Amélioration mise à jour des commandes

#### Version 20201105

- Correction affichage chiffre pour les seuils et l'offset https://community.jeedom.com/t/pas-dalerte-givre/41213/8?u=jag

#### Version 20201031

- Amélioration de la liste des objets parents

#### Version 20201027

- Amélioration Visu sur dashboard

#### Version 20201026

- Amélioration création des commandes
- Amélioration mise à jour des commandes
- Modification affichage des commandes
- Ajout BP reset de recherche
- Clean Log + code
- Correction Bug Rosee \_eqNameID (erreur de TEST)
- Correction bug suppression commande Refresh
- Correction Warning PHP
- Correction variable non défini
- Amélioration si pb historique pression
- Correction Bug création des commandes

#### Version 20200525

- Correction Bug Recréation des commandes
- Fin clean suite à déplacement de la documentation
- Amélioration code (gestion affichage de paramètres suivant le mode de calcul)

#### Version 20200512

- Déplacement documentation
- Correction bug enregistrement individuel de chaque équipement
- Enregistrement des équipements après chaque mise à jour
- Modification widget pour la tendance

#### Version 20200430

- Correction ajout widget Core par défaut sur les nouveaux équipements

#### Version 20200418

- Ajout calcul "Tendance Météo"
- Nettoyage log
- Corrections bugs
- Corrections bug sur le choix d'équipement obligatoire
- Ajout Cron 10/15/Heures
- Remplacement Cron5 par Cron30 (les calculs se feront par défaut toutes les 30 minutes)
  > **Info : Penser à vérifier que le Cron 30 est actif sinon il faut l'activer**
- Ajout widget Core pour les commandes (uniquement pour les nouveaux équipements)
- Ajout widget pour la tendance (uniquement pour le Core V4 et les nouveaux équipements)

#### Version 20200409

- Séparation des calculs
- Nettoyage des infos dans les logs
- Ajout bouton pour recréer les commandes
- Résolution Bug Liste déroulante choix calcul vide
- Masquage des paramètres non nécessaire suivant le mode de calcul
- Modification création des commandes cela tient compte désormais du mode de calcul
- Suppression de certains calculs intermédiaires
- Affectation valeur Min et Max sur le "Message numérique"

> Info : Penser à sauvegarder chaque équipement

#### Version 20200226

- Le point de givre est égal à 5 si la température dépasse 5°
- Possibilité de sélectionner uniquement une partie du calcul (Rosée et givre, Humidité absolue, Givre, Point de rosée)
- Ajout offset sur la température (valeur par défaut : 0)

#### Version 20200210

- Le point de givre est égal à la température quand la température est supérieure à 10°C

#### Version 20200209

> _Info : Changement de l'auteur du plugin, merci @claude.metzger_

- Ajout de log supplémentaire en mode DEBUG
- Nettoyage du code
- Nouveau calcul pour la gestion de l'alerte givre
- Ajout d'un message pour le type de givre ainsi que d'une valeur numérique suivant le code <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue</a>
  > - CAS N°0 : Message = _Aucun risque de Givre_, Alerte givre = _0_, Message numérique = _0_
  > - CAS N°1 : Message = _Givre peu probable malgré la température_, Alerte givre = _1_, Message numérique = _1_
  > - CAS N°2 : Message = _Risque de givre_, Alerte givre = _1_, Message numérique = _2_
  > - CAS N°3 : Message = _Givre, Présence de givre_, Alerte givre = _1_, Message numérique = _3_
- Changement du logo du plugin merci @mich0111
- Correction type de générique
- Possibilité d'enregistrer l'équipement sans les champs obligatoires si l'équipement n'est pas actif
- Modification affichage des commandes
  > - Ajout la possibilité d'inverser les commandes binaires
  > - Suppression de l'historique sur les commandes messages
- Ajout des nouvelles commandes en automatique sans recréer les commandes (Merci à Kiboost et à Mips)
- Modification du type de données pour les seuils => Uniquement numérique
- Ajout d'un seuil d'humidité absolue pour le calcul de l'alerte de givre
- Pas de calcul des infos de givres si la température est supérieure à 10°C

  > _Remarque : Il est obligatoire de sauvegarder chaque équipement pour avoir les nouvelles commandes_


### <2020

#### Version 3.3.2

- Ajout de log supplémentaire en mode DEBUG
- Suppression visibilité pour le calcul du point de rosée et du point de givrage

#### Version 3.3.1

- Correction Documentation

#### Version 3.3

- Correction Bug

#### Version 3.2

- Ajout d’un Cron 30 (Merci à kiboost)
- Amélioration de l'affichage pour le Core V4 (Merci à kiboost)
- Possibilité de renommer les commandes (Merci à kiboost)
- Correction des historiques (Merci à kiboost)
- Commande Refresh (sur la tuile, scénario etc) (Merci à kiboost)
- Amélioration des logs
- Correction type de Generic
- Correction Bug : l'actualisation des données ne se fait plus si l'équipement est désactivé
- Les alertes sont visible par défaut (plus de masquage si l'alerte est à 0)
- Nettoyage des dossiers (Merci à kiboost)
- Mise à jour de la documentation

> _Remarque : Il est conseillé de supprimer le plugin et ensuite le réinstaller_

#### Version 3.1

- La recherche des cmd pour mise à jour ne se fait plus par getConfiguration('data') mais par leur logicalId. Les cmd perdent leur data de configuration. (merci à jpty)

#### Version 3.0

- Support de PHP 7.3
- Migration vers font-awesome 5
- Migration affichage au format core V4

#### Version 2.1

- Correction affichage point de rosée et givres défaillants

#### Version 2.0

- Mise à jour pour compatibilité V3 Jeedom

#### Version 1.5.2

- Correction de bug dans rosee.class.php dans l'appel de la fonction cron15() (merci à mika-nt28 et Mika)

#### Version 1.5.1

- Correction de bug dans la prise en compte du seuil d’alerte rosée

#### Version 1.5

- Gestion des alertes rosée et givre par changement d’état (merci Toregreb)

#### Version 1.4

- Seuil d’alerte du point de rosée configurable dans Informations. Valeur par défaut 2°C

#### Version 1.3.1

- Réglage du seuil d’alerte du point de rosée et du point de givrage à 2°C (dépression du point de rosée)

#### Version 1.3

- Ajout d’une alerte point de rosée et d’une alerte point de givrage

#### Version 1.2

- Sélection de la température et de l’humidité (possibles par un bouton de recherche) (merci Lunarok)

#### Version 1.1

- Ajout du point de givre

#### Version 1.0

- Création du plugin
