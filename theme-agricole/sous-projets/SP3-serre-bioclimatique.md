# SP3 — Serre bioclimatique adaptée au climat tropical

> Concevoir un espace de culture protégé qui régule passivement sa température.

## Déclinaison MEI

### Matière
- Maquette de serre à échelle réduite
- Structure résistante au vent (conception + matériaux)
- Choix de couverture : diffusion lumineuse, filtre UV
- Système d'ouverture (ouvrants motorisés)

### Énergie
- Étude thermique simplifiée (apports solaires, ventilation naturelle)
- Motorisation des ouvrants (servomoteurs)
- Bilan énergétique global

### Information
- Capteurs intérieurs : température, humidité, luminosité
- Automate de pilotage des ouvrants selon conditions
- Remontée de données vers le dashboard

## Défis techniques
- Ventilation naturelle suffisante sans climatisation
- Résistance aux rafales
- Compromis lumière/chaleur en climat tropical

## Technologies clés
- Arduino/ESP32, DHT22, BH1750, servomoteurs
- Impression 3D pour la structure de maquette
- MQTT

## Ancrage Martinique
- Serre tropicale ≠ serre tempérée (l'enjeu est de refroidir, pas de chauffer)
- Protection contre les pluies battantes
- Ventilation croisée adaptée aux alizés

## Interconnexions MQTT
- **Publie :** `ferme/serre/temperature`, `ferme/serre/humidite`, `ferme/serre/luminosite`, `ferme/serre/ouvrants`
- **Consomme :** `ferme/meteo/temperature`, `ferme/meteo/vent`

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
