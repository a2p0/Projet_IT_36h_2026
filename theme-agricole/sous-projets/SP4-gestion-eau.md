# SP4 — Gestion de l'eau : collecte, stockage et qualité

> Récupérer l'eau de pluie, la stocker et surveiller sa qualité pour l'exploitation.

## Déclinaison MEI

### Matière
- Maquette du système de collecte (toiture, gouttières, filtration primaire, cuve)
- Dimensionnement du stockage selon pluviométrie locale
- Choix de matériaux (cuve, filtres)

### Énergie
- Pompe de relevage (dimensionnement)
- Bilan énergétique du traitement (filtration, UV éventuel)

### Information
- Capteurs de niveau de cuve (ultrason)
- Capteur de turbidité
- Suivi de consommation, alertes niveau bas
- Publication MQTT

## Défis techniques
- Dimensionnement réaliste basé sur données pluviométriques de Martinique
- Filtration adaptée aux eaux de ruissellement tropicales
- Fiabilité du capteur de niveau

## Technologies clés
- Arduino/ESP32, HC-SR04 (niveau), capteur de turbidité, pompe miniature
- Relais, électrovanne
- MQTT

## Ancrage Martinique
- Alternance carême/hivernage : gestion saisonnière de la ressource
- Dépendance à l'eau de réseau coûteuse
- Récupération d'eau de pluie comme levier d'autonomie

## Interconnexions MQTT
- **Publie :** `ferme/eau/niveau_cuve`, `ferme/eau/turbidite`, `ferme/eau/consommation`
- **Consomme :** `ferme/meteo/pluie` (SP1)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
