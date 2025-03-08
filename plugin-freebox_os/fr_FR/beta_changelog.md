# Plugin Freebox_OS

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />

## Info Changelog BETA

### Important

> **_Pour rappel_**, s'il n'y a pas d'information sur la mise à jour, c'est que celle-ci concerne uniquement de la mise à jour de documentation, de traduction ou de corrections de bugs mineurs.
>
> **Attention : Il est nécessaire d'avoir la Freebox serveur en version 4.8.18 pour que le plugin fonctionne.**

### Fil d'actualité

> [Voir le fil d'actualité du plugin sur Community](https://community.jeedom.com/t/info-plugin-freebox-mise-a-jour-des-composants-de-la-delta-tiles-systeme/30673)

## 2025

## 08/03/2025

- **Player**
- Ajout fonction Mute (son)
- Ajour fonction changer le volume
- Ajout Fonction du contrôle du volume

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**
> **Les nouvelles commandes sont créées uniquement si le player est joignable**
> **Pour l'instant, il n'est pas possible de changer de chaîne**

## 09/02/2025

- Amélioration log et message pour l'erreur de cron "Ajout des nouvelles commandes" des appareils connectés

## 06/02/2025

- Changement nom icône pour la documentation

## 29/01/2025

- Correction version API en cas de reset : Passage de V10 à v13
- Correction bouton "Lancement de l'authentification"
- Changement dépot Plugin > [Voir GITHUB](https://github.com/JEALG/Jeedom-Freebox_OS)
- Changement icône Plugin

## 28/01/2025

- Migration de l'API mini en v13.

### 27/01/2025

- **Wifi**
- Ajout commande "Choix Mode de veille planning" pour le wifi pour les box compatibles avec le mode Eco Wifi

- **Community**
- Ajout info supplémentaire pour Community

- **Scan équipements standards**
- Correction création des équipements de type VM sur les freebox non compatible

> [Voir le sujet sur communnity](https://community.jeedom.com/t/api-non-compatible-avec-les-vm-sur-les-freebox-revolution/137141?u=jag)

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**

### 26/01/2025

- Mise à jour des liens des images

### 12/01/2025

- Mise à jour des liens des images

- **Wifi**
- Ajout Etat mode eco Wifi (pour les freebox compatibles)
- Mise à jour des noms des commandes de l'état des cartes Wifi (suivant les cas, il faut lancer 2 fois la recherche)
- Correction retour Etat WPS

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**

### 05/01/2025

- Amélioration changement Nom des commandes pour les appareils connectés

### 01/01/2025

- Corrections log

## 2024

### 23/12/2024

- **Ensemble des équipements standards**
- Ajout vérification si présence disque

- **Système**
- Ajout l'état du disque dans l'équipement système

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**

### 15-16/12/2024

- **Ensemble des équipements standards**
- Ajout vérification si la box est compatible avec les VM
- Ajout vérification si la box est compatible avec les différents type d'affichage de l'écran de la box

- **Afficheur LCD**
- Correction commande off pour l'orientation
- Correction de la commande Lumininosité écran
- Ajout gestion Freebox Ultra Edition 25
- Correction de la valeur de la position du texte pour l'afficheur

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**

### 13/11/2024

- Correction création commande du Player (il faut relancer une recherche pour de nouveau avoir l'état)
- Correction création commande du Wifi

### 12/11/2024

- Amélioration log

- **Téléphone**
- Ajout des commandes pour uniquement les nouveaux appel manqués et reçus
- Correction bug si la liste est vide
- Correction traduction

### 11/11/2024

- Correction création disque
- Correction requête pour le téléphone

### 10/11/2024

- Correction bug bouton lancement de l'authentification

### 11/10/2024

- Correction bug bouton lancement de l'authentification
- Correction type de regroupement d'appareil pour les débits
- Correction du demon : il sera redemarré uniquement si l'authentification a été faite lors de la première installation.

### 27/09/2024

- Correction bug installation depuis Market

### 20 et 25 /09/2024

- Correction bug setConfiguration sur la création des commandes
- Traduction
- Ajout Firmware dans le lien communauty
- Clean code
- Correction PHP 8
- Traduction
- Core mini 4.2
- Traitement fonction Deprecated

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS ET PARENTAL**

### 05/09/2024

- Correction PHP 8
- Correction bug remise a zéro téléphonie

### 23/08/2024

- Correction bug authentification

### 21/08/2024

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS ET PARENTAL**

- **Ensemble des équipements standards**

- Reprise de l'ensemble des mises à jour
- Amélioration info vers Community pour le Core 4.4

- **Contrôle parental**

- Ajout commande pour "appareil associé"
- Ajout commande pour "Vacances associées au profil"

> **ATTENTION : Il faudra supprimer la commande ETAT et renommer ETAT(1) en ETAT**

- **Afficheur**

- Ajout commandes pour forcer l'orientation
- Ajout commandes pour cacher la clef Wifi

- **Systeme**

- Ajout commande info sur la mise à jour du firmware de la Freebox Serveur avec les valeurs suivantes
      - Le processus de mise à jour est en cours d\'initialisation
      - Le micrologiciel est en cours de mise à jour
      - Le micrologiciel est à jour
      - Une erreur s'est produite pendant la mise à jour
- Ajout info de la langue d'affichage

- **Wifi**
- Ajout Info du type de mode Eco pour le wifi
- Ajout du mode de veille pour la planification du Wifi
