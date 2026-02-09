# SP7 — Système anti-nuisibles et protection des cultures

> Détecter et dissuader les ravageurs sans produits chimiques.

## Déclinaison MEI

### Matière
- Conception de pièges/barrières physiques (impression 3D)
- Boîtier étanche pour l'électronique de détection
- Structure de montage sur piquet/poteau

### Énergie
- Alimentation autonome (petit panneau solaire + batterie)
- Actionneurs de dissuasion : buzzer, LED stroboscopique, servomoteur

### Information
- Détection de présence (capteur PIR, ultrason)
- Comptage d'événements et horodatage
- Alertes MQTT, historique pour identifier les horaires critiques

## Défis techniques
- Discrimination simplifiée entre nuisibles et animaux utiles
- Fonctionnement nocturne fiable
- Résistance aux intempéries tropicales

## Technologies clés
- ESP32, PIR HC-SR501, HC-SR04, buzzer, LED haute puissance
- Panneau solaire 5W, batterie, servomoteur
- MQTT, JSON

## Ancrage Martinique
- Problématique des ravageurs tropicaux (rats, mangoustes, insectes)
- Mouvement vers le zéro-phyto (héritage chlordécone)
- Agriculture biologique en développement

## Interconnexions MQTT
- **Publie :** `ferme/protection/alertes`, `ferme/protection/compteur`, `ferme/protection/etat`
- **Consomme :** `ferme/meteo/luminosite` (SP1, pour contextualiser jour/nuit)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
