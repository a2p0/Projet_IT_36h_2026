# SP8 — Supervision centralisée et affichage dynamique

> Agréger les données de tous les modules et les rendre visibles pour la communauté scolaire.

## Déclinaison MEI

### Matière
- Boîtier de la station centrale (Raspberry Pi + écran)
- Signalétique physique (panneau d'affichage avec voyants d'état par module)
- Conception ergonomique

### Énergie
- Alimentation sécurisée avec batterie de secours
- Bilan de consommation du système de supervision

### Information
- Broker MQTT (Mosquitto sur Raspberry Pi)
- Dashboard Node-RED
- Stockage de données (InfluxDB ou CSV)
- Écran d'affichage dynamique (infos campus temps réel)
- Logique d'alertes, accès mobile

## Défis techniques
- Intégration de tous les flux de données des 7 autres groupes
- Interface lisible et attractive pour un public scolaire
- Fiabilité 24/7

## Technologies clés
- Raspberry Pi 4, Mosquitto, Node-RED, InfluxDB
- Écran tactile 7" ou moniteur HDMI
- Python pour scripts, MQTT, HTML/CSS pour l'affichage

## Ancrage Martinique
- Communication interne dans les établissements antillais
- Résilience aux coupures (mode dégradé offline)
- Valorisation des initiatives durables auprès de la communauté éducative

## Interconnexions MQTT
- **Publie :** `campus/systeme/etat`, `campus/systeme/alertes`
- **Consomme :** tous les topics de tous les autres modules

## Rôle particulier

Comme pour le thème agricole, ce groupe a un rôle transversal et doit piloter la définition du protocole MQTT commun en début de projet. Ce groupe doit être constitué d'élèves autonomes et communicants.

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
