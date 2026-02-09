# SP2 — Fontaines à eau connectées et économes

> Fournir de l'eau fraîche en libre-service tout en surveillant la consommation et la qualité.

## Déclinaison MEI

### Matière
- Maquette d'une fontaine (circuit hydraulique simplifié, buse, bac de récupération)
- Choix de matériaux alimentaires
- Design hygiénique (sans contact)

### Énergie
- Système de refroidissement (module Peltier ou circulation)
- Bilan thermique en climat tropical
- Consommation énergétique du refroidissement

### Information
- Compteur de volumes distribués (débitmètre)
- Capteur de température de l'eau
- Détection de présence (distribution sans contact)
- Suivi de consommation sur le dashboard

## Défis techniques
- Refroidissement efficace malgré 30°C ambiants
- Hygiène sans contact
- Consommation énergétique maîtrisée

## Technologies clés
- Arduino/ESP32, module Peltier TEC1-12706, capteur DS18B20, débitmètre YF-S201
- Capteur IR (sans contact), pompe miniature
- MQTT

## Ancrage Martinique
- Hydratation critique en climat tropical
- Réduction des bouteilles plastiques
- Qualité de l'eau courante en Martinique

## Interconnexions MQTT
- **Publie :** `campus/fontaine/temperature_eau`, `campus/fontaine/volume`, `campus/fontaine/etat`
- **Consomme :** `campus/energie/disponibilite` (SP7)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
