# Interface wifi web **autonome** ou **HA** pour **Diverter**
Vous trouverez ici une configuration yaml pour esphome qui permet de prendre le controle d'un diverter via wifi.

- [Introduction](#Introduction)
- [Fonctionnalités](#Fonctionnalités)
- [Prérequis](#Prérequis)
- [Instructions d'installation](#Instructions-d'installation)

---

## Introduction
**Autonome** par défaut

Cette solution vous permet de contrôler votre **diverter** directement via **Wi-Fi** en tant que composant autonome. Cette solution n'a pas besoin **d'Home Assistant**, mais si vous préférez, vous pouvez utiliser **Home Assistant**. Avec le composant **ESPHome**, l'ajout du composant sera automatique.

Pour plus d'informations sur le **diverter**, veuillez suivre ce lien : [http://wikinid.free.fr/wiki/Main/DiverterModule](http://wikinid.free.fr/wiki/Main/DiverterModule)

---

## Fonctionnalités
**Remontée** d'infos et programmation des **plages horaires** de marche forcée..

Vous pouvez contrôler votre **diverter** depuis une interface **Web**. Elle affichera les informations de puissance principales. Elle permet de prendre le **contrôle** de la marche forcée en programmant les plages horaires de marche forcée.

## Aperçu de l'interface web accessible en autonome

<img src="https://raw.githubusercontent.com/lcailler/diverter2esphome/refs/heads/main/screenshot00.png" width="600">

---

## Prérequis
**Sonoff** ou tout autre appareil compatible **ESPHome**

La configuration disponible ici est adaptée à un [Sonoff Basic R2](https://devices.esphome.io/devices/Sonoff-BASIC-R2-v1.4).
Avec quelques adaptations **mineures**, vous pourrez adapter cette configuration.

---

## Instructions d'installation

### installation esphome

Plusieurs façons pour installer esphome sur votre carte esp8266 ou autre. Cela peut être via home assistant mais aussi directement depuis votre pc.

Concrètement, sous home assistant, ajouter le composant "ESPHome Device Builder", puis ouvrir "l'interface utilisateur web". Voici un guide : https://www.hacf.fr/esphome-introduction/

### flash du firmware

Avec ESPHome flasher le firmware basee sur le fichier yaml suivant : sonoff-esp-diverter.yaml & secrets.yaml

### première mise sous tension :

Pas d'obligation de renseigner vos paramètres Wi-Fi dans la configuration.
Une fois flashé, si votre configuration Wi-Fi n'est pas faite, un hotspot Wi-Fi est activé. Connectez-vous sur ce hotspot et configurez votre Wi-Fi local, ssid et password.



