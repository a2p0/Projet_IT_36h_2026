# SP6 — Robot d'assistance agricole mobile

> Concevoir un petit robot mobile capable de se déplacer entre les parcelles pour des tâches simples.

## Déclinaison MEI

### Matière
- Châssis adapté au terrain (roues larges ou chenilles pour sol meuble)
- Structure résistante aux projections d'eau
- Conception CAO + impression 3D

### Énergie
- Motorisation (2-4 moteurs DC avec drivers)
- Alimentation batterie, étude d'autonomie
- Recharge possible via SP5

### Information
- Pilotage (télécommande ou suivi de ligne)
- Capteur ultrason anti-collision
- Caméra optionnelle, remontée de position

## Défis techniques
- Mobilité sur terrain meuble et irrégulier
- Autonomie suffisante pour un parcours utile
- Robustesse mécanique du châssis

## Technologies clés
- Arduino Mega / ESP32, L298N, moteurs DC, HC-SR04
- Batterie Li-ion, capteur de ligne (IR)
- Impression 3D pour châssis, MQTT

## Ancrage Martinique
- Main-d'œuvre agricole rare en Martinique
- Petites parcelles nécessitant des engins légers et agiles
- Terrain volcanique meuble et parfois pentu

## Interconnexions MQTT
- **Publie :** `ferme/robot/position`, `ferme/robot/batterie`, `ferme/robot/etat`
- **Consomme :** `ferme/meteo/pluie` (arrêt si forte pluie)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
