# SP1 — Station agro-météo connectée

> Collecter et diffuser les données climatiques locales pour piloter l'ensemble de l'exploitation.

## Déclinaison MEI

### Matière
- Conception et fabrication d'un abri météo ventilé (impression 3D / découpe)
- Résistant aux UV et à l'humidité tropicale
- Fixation robuste (vent)

### Énergie
- Alimentation solaire autonome (petit panneau + batterie)
- Dimensionnement pour fonctionnement 24/7
- Régulation de charge

### Information
- Acquisition multicapteurs : température, humidité air, pluviométrie, anémomètre, UV
- Transmission MQTT vers le broker central
- Affichage sur le dashboard commun

## Défis techniques
- Précision des mesures en environnement tropical humide
- Protection IP65 de l'électronique
- Autonomie énergétique réelle

## Technologies clés
- ESP32, DHT22/BME280, BH1750, anémomètre, pluviomètre
- Panneau solaire 5-10W, batterie Li-ion, régulateur TP4056
- MQTT, JSON

## Ancrage Martinique
- Paramètres critiques pour l'agriculture antillaise (indice UV, alertes cycloniques)
- Suivi des transitions carême/hivernage
- Données pluviométriques locales comme référence

## Interconnexions MQTT
- **Publie :** `ferme/meteo/temperature`, `ferme/meteo/humidite`, `ferme/meteo/pluie`, `ferme/meteo/vent`, `ferme/meteo/uv`
- **Consomme :** aucun (module source)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
