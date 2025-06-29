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

### 06/05/2025

- Correction API non disponible pour les Players [Sujet community](https://community.jeedom.com/t/freebox-os-messages-derreur-depuis-la-derniere-mise-a-niveau/140390?u=jag)
- Correction message d'erreur pour les modules 4G non disponible [Sujet community](https://community.jeedom.com/t/error-message-inconnue-noent/140388?u=jag)

> **ATTENTION : Le plugin remonte maintenant plus de problème de communication entre Jeedom et la Freebox**
> **ATTENTION : DERNIERE VERSION DU PLUGIN COMPATIBLE AVEC DEBIAN 10**

### 05/05/2025

- Correction erreur avec PHP <8 [Sujet community](https://community.jeedom.com/t/call-to-undefined-function-str-contains/140353/9)

> **ATTENTION : DERNIERE VERSION DU PLUGIN COMPATIBLE AVEC DEBIAN 10**

### 26/04/2025

- **Player**
- Ajout une commande pour lancer les chaines
- Amélioration de la disposition des boutons sur le dashboard
- Amélioration mise à jour des commandes
- Correction Warning PHP et bugs
- Amélioration création des commandes
- Ajout date de la derniere fois que le player a été vue sur le réseau
- Ajout fonction Mute (son)
- Ajour fonction changer le volume
- Ajout info numéro de chaîne
- Ajour info nom de la chaîne
- Ajout de l'adresse IP4 dans l'équipement du player
- Ajout commmande multiple :
      - Ouvrir le menu "Replay"
      - Ouvrir le menu "Radio"
      - Ouvrir Netfix, Prime Vidéo, Youtube, Mes enregistrements
      - Allumer le player avec la dernière chaine ouverte
- Possibilité de redémarrer le player

> [Merci a ce site](https://github.com/Aymkdn/assistant-freebox-cloud/wiki/Player-API)
> [Merci a cette issue](https://github.com/JEALG/Jeedom-Freebox_OS/issues/446)
> **ATTENTION : IL FAUT RELANCER UNE RECHERCHE DES EQUIPEMENTS STANDARDS**
> **Les nouvelles commandes sont créées uniquement si le player est joignable**
 **Il faut absolument que le Player soit sous tension et pas en veille prolongée (Révolution) lors de la recherche**

- **Appareils connectés**
- Correction warning PHP

- **Freeplugs**
- Ajout d'info sur les Freeplugs

- **Partage Windows Mac**
- Ajout d'info dans le Partage Windows - Mac

- **Global**
- Amélioration mise à jour requête sur la Freebox
- Amélioration retour info d'erreur de requête

> [Merci a cette issue](https://github.com/JEALG/Jeedom-Freebox_OS/issues/446)