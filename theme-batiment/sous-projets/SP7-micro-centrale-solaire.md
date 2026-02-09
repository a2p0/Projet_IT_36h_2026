# SP7 — Micro-centrale solaire du bâtiment avec suivi énergétique

> Produire et monitorer l'énergie renouvelable à l'échelle du bâtiment scolaire.

## Déclinaison MEI

### Matière
- Maquette de toiture avec panneaux solaires intégrés
- Support et inclinaison optimisée (latitude 14.6°N)
- Câblage et connectique

### Énergie
- Dimensionnement réaliste (bilan des consommations du bâtiment)
- Surface de panneaux nécessaire, stockage, régulation
- Taux d'autoconsommation

### Information
- Monitoring temps réel de la production et de la consommation
- Calcul du taux d'autoconsommation
- Historique et tendances
- Affichage pédagogique (écran dans le hall)

## Défis techniques
- Bilan énergétique réaliste du bâtiment
- Dimensionnement cohérent et crédible
- Visualisation claire des flux d'énergie (production vs consommation)

## Technologies clés
- Panneau solaire 20-50W, régulateur MPPT, batteries
- ESP32, INA219, capteur de courant ACS712
- MQTT, Node-RED pour dashboard énergétique

## Ancrage Martinique
- Objectif d'autonomie énergétique insulaire
- Coût élevé de l'électricité (tarifs EDF Martinique)
- Sensibilisation des élèves à la transition énergétique

## Interconnexions MQTT
- **Publie :** `campus/energie/production`, `campus/energie/consommation`, `campus/energie/batterie`, `campus/energie/disponibilite`
- **Consomme :** consommations déclarées par les autres modules

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
