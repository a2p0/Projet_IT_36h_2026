# SP3 — Distributeur connecté éco-responsable

> Concevoir un distributeur de boissons/snacks à faible impact environnemental.

## Déclinaison MEI

### Matière
- Mécanisme de distribution (spirale ou gravité, servomoteur)
- Structure du distributeur en maquette
- Choix de matériaux recyclables

### Énergie
- Réfrigération basse consommation
- Alimentation solaire possible, mode veille intelligent
- Bilan énergétique

### Information
- Interface utilisateur (écran LCD + boutons ou RFID)
- Gestion des stocks (capteurs de niveau/poids)
- Alertes de réapprovisionnement
- Suivi des distributions

## Défis techniques
- Fiabilité du mécanisme de distribution
- Gestion du froid en ambiance chaude
- Interface intuitive

## Technologies clés
- Arduino/ESP32, servomoteurs, LCD I2C, RFID RC522
- Capteur de poids (HX711 + cellule de charge), module Peltier
- MQTT

## Ancrage Martinique
- Promotion de produits locaux (jus de fruits pays, snacks artisanaux)
- Réduction des emballages, économie circulaire
- Chaleur ambiante : conservation des produits

## Interconnexions MQTT
- **Publie :** `campus/distributeur/stock`, `campus/distributeur/ventes`, `campus/distributeur/temperature`
- **Consomme :** `campus/energie/disponibilite` (SP7)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
