# SP8 — Tableau de bord central et système d'alerte

> Agréger toutes les données de l'exploitation et fournir une aide à la décision à l'agriculteur.

## Déclinaison MEI

### Matière
- Boîtier de la station centrale (Raspberry Pi + écran)
- Conception ergonomique
- Signalétique visuelle (voyants LED d'état par module)

### Énergie
- Alimentation sécurisée avec batterie de secours
- Bilan de consommation de la station centrale

### Information
- Serveur MQTT (broker Mosquitto)
- Interface web Node-RED
- Stockage des données (InfluxDB ou fichiers CSV)
- Logique d'alertes (seuils, combinaisons multi-capteurs)
- Notification (email, signal lumineux)

## Défis techniques
- Intégration des protocoles de tous les autres groupes
- Fiabilité du système central (c'est le point unique de défaillance)
- Interface utilisateur intuitive pour un agriculteur non-technicien

## Technologies clés
- Raspberry Pi 4, Mosquitto, Node-RED, InfluxDB
- Écran tactile 7", LEDs de signalisation
- Python pour scripts d'alerte, MQTT

## Ancrage Martinique
- Accès à distance pour l'agriculteur (smartphone)
- Fonctionnement en mode dégradé (coupures internet/électricité fréquentes)
- Interface simple adaptée à un public non-technophile

## Interconnexions MQTT
- **Publie :** `ferme/systeme/etat`, `ferme/systeme/alertes`
- **Consomme :** tous les topics de tous les autres modules

## Rôle particulier

Ce sous-projet a un rôle central et transversal : le groupe SP8 doit collaborer activement avec tous les autres groupes pour définir les conventions de communication. Il est recommandé de démarrer ce sous-projet en même temps que les autres et de mener la phase de définition du protocole MQTT commun.

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
