# SP6 — Ombrières dynamiques pour la cour

> Concevoir des structures d'ombrage motorisées qui s'adaptent au soleil et aux conditions météo.

## Déclinaison MEI

### Matière
- Maquette d'ombrière à voile rétractable ou orientable
- Structure, toile, axes de rotation
- Résistance au vent, étude des matériaux

### Énergie
- Motorisation de l'orientation/rétraction (servomoteurs)
- Possibilité d'intégrer des panneaux solaires souples sur la voile
- Bilan énergétique

### Information
- Capteur de luminosité et de vent
- Algorithme de positionnement automatique
- Rétraction de sécurité en cas de vent fort (mode cyclonique)
- Remontée d'état vers le dashboard

## Défis techniques
- Résistance mécanique au vent
- Motorisation fiable et silencieuse
- Automatisme de sécurité (repli cyclonique rapide)

## Technologies clés
- Arduino/ESP32, servomoteurs MG996R, anémomètre, BH1750
- Impression 3D (articulations), matériaux textiles
- MQTT

## Ancrage Martinique
- Protection solaire indispensable dans les cours antillaises
- Risque cyclonique imposant des structures rétractables
- Confort thermique extérieur (réduction de la température ressentie)

## Interconnexions MQTT
- **Publie :** `campus/ombriere/position`, `campus/ombriere/etat`, `campus/ombriere/vent`
- **Consomme :** aucun (capteurs propres), possibilité de partage météo avec d'autres SP

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
