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

### 31/12/2025

- Amélioration des messages d'erreur

### 21/10/2025

- Amélioration Log pour la partie recherche disque

### 08/10/2025

- Correction groupe équipement pour la partie domotique

### 04/10/2025

- Correction Warning PHP

### 22/09/2025

- **Wifi**
- Amélioration commande WIFI

### 19/09/2025

- **Wifi**
- Ajout de la liste des appareils connectés par carte WIFI

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**

### 12/08/2025

- **Global**
- Correction Cron qui se modifie à chaque recherche des équipements
- Migration de l'API mini en v14

- **VM**
- Correction requête VM (trop de / dans la requête)
- Correction de la désactivation de l'équipement VM
- Correction action "stop" - " Redémarrer" - "start"

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**
>
> **Si le scan n'est pas fait, vous aurez peut être le message suivant :** La version de l'API n'est pas compatible ───▶︎ Code Erreur = invalid_api_version

### 15/07/2025

- Traitement de l'erreur "Nodev" en mode Debug uniquement (Adresse mac introuvable)
- Gestion du mode bridge pour ne pas récupèrer certaines information du player

### 06/07/2025

- Suite amélioration de l'équipement Gestion du réseau
- Correction Bug liste des équipements réseaux 


### 29/06/2025

- Réecriture de la mise à jour et action de l'équipement Gestion du réseau

> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**

### 24/05/2025

- Amélioration récupération des données
- Afficheur possiblité d'éteindre la LED pour les box compatibles
- Correction Bug récupération données Freeplug

### 19/05/2025

- Amélioration Contrôle parental
- Amélioration mise à jour de la partie système
- Correction Bug Variable par défaut lors de la mise a jour

### 18/05/2025

- Amélioration Contrôle parental
- Amélioration retour info etat Wifi

### 11/05/2025

- Amélioration Player (clean code + non création des commandes si la variable n'existe pas)