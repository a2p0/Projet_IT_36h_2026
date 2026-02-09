# SP4 — Espace détente intelligent

> Créer un espace de bien-être pour les élèves avec ambiance adaptative.

## Déclinaison MEI

### Matière
- Maquette de l'espace (mobilier modulable, cloisons acoustiques simplifiées)
- Ergonomie et confort
- Choix de matériaux absorbants (bruit)

### Énergie
- Éclairage LED à intensité et température de couleur variables
- Ventilation basse consommation
- Bilan énergétique de la salle

### Information
- Capteur de fréquentation (comptage entrées/sorties)
- Capteur de bruit (microphone + traitement niveau sonore)
- Régulation automatique de l'ambiance (lumière, ventilation)
- Affichage du taux d'occupation

## Défis techniques
- Régulation multi-paramètres (bruit, lumière, température)
- Comptage fiable des personnes
- Créer une ambiance réellement apaisante

## Technologies clés
- ESP32, capteur sonore, PIR ou barrière IR (comptage), DHT22
- LED RGB (NeoPixel), ventilateur PWM
- MQTT, Node-RED pour le pilotage d'ambiance

## Ancrage Martinique
- Bien-être des élèves en milieu scolaire tropical
- Gestion du bruit dans les bâtiments ouverts (pas d'isolation naturelle)
- Pause méridienne longue aux Antilles : besoin d'espaces de repos

## Interconnexions MQTT
- **Publie :** `campus/detente/frequentation`, `campus/detente/bruit`, `campus/detente/ambiance`
- **Consomme :** aucun

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
