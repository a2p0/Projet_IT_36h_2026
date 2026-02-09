# SP5 — Station de recharge solaire pour appareils mobiles

> Offrir des points de recharge alimentés par énergie solaire dans les espaces communs.

## Déclinaison MEI

### Matière
- Structure de la station (poteau, support de panneau, boîtier de prises)
- Design résistant aux intempéries et au vandalisme
- Matériaux anti-corrosion

### Énergie
- Panneau solaire, régulateur de charge, batterie tampon
- Dimensionnement pour N ports USB simultanés
- Rendement et autonomie quotidienne

### Information
- Monitoring de production/consommation
- Affichage en temps réel (énergie produite, disponibilité des ports)
- Gestion de priorité de charge
- Données vers le dashboard

## Défis techniques
- Dimensionnement réaliste (combien de téléphones par jour ?)
- Sécurité électrique (USB 5V)
- Résistance extérieure (pluie, soleil, vandalisme)

## Technologies clés
- Panneau solaire 10-20W, régulateur, batterie Li-ion
- ESP32, INA219 (monitoring), écran OLED
- Modules step-down 5V, connecteurs USB
- MQTT

## Ancrage Martinique
- Fort ensoleillement valorisé directement par les élèves
- Sensibilisation concrète aux énergies renouvelables
- Besoin réel : téléphones déchargés en fin de journée

## Interconnexions MQTT
- **Publie :** `campus/recharge/production`, `campus/recharge/consommation`, `campus/recharge/ports_dispo`
- **Consomme :** aucun (autonome)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
