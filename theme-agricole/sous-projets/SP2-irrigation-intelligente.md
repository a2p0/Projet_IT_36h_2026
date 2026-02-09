# SP2 — Irrigation intelligente et économe

> Optimiser l'arrosage en fonction de l'état réel du sol et des prévisions météo.

## Déclinaison MEI

### Matière
- Réseau d'irrigation en maquette (tuyaux, goutteurs, électrovannes)
- Choix de matériaux résistants aux UV
- Conception du circuit hydraulique

### Énergie
- Dimensionnement de la pompe et des électrovannes
- Bilan énergétique du système
- Alimentation depuis le réseau solaire (SP5)

### Information
- Capteurs d'humidité du sol en plusieurs points
- Algorithme de décision (seuils adaptatifs)
- Intégration des données météo du SP1 via MQTT

## Défis techniques
- Calibration des capteurs en sol volcanique
- Gestion de zones d'arrosage différenciées
- Algorithme de décision multi-paramètres

## Technologies clés
- Arduino/ESP32, capteurs d'humidité du sol capacitifs, électrovannes 12V
- Relais, pompe miniature
- MQTT pour consommation des données météo

## Ancrage Martinique
- Stress hydrique en carême : économie d'eau critique
- Sols volcaniques à drainage rapide
- Coût de l'eau en contexte insulaire

## Interconnexions MQTT
- **Publie :** `ferme/irrigation/humidite_sol`, `ferme/irrigation/etat_vannes`, `ferme/irrigation/volume`
- **Consomme :** `ferme/meteo/pluie`, `ferme/meteo/temperature`, `ferme/eau/niveau_cuve` (SP4)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
