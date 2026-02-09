# SP1 — Accessibilité PMR intelligente

> Faciliter le déplacement des personnes à mobilité réduite grâce à un guidage connecté.

## Déclinaison MEI

### Matière
- Maquette d'un parcours accessible (rampe motorisée ou porte automatique à échelle réduite)
- Conformité dimensionnelle aux normes PMR
- Choix de matériaux (solidité, esthétique)

### Énergie
- Motorisation des ouvrants (servomoteur/vérin)
- Dimensionnement et consommation
- Alimentation sécurisée

### Information
- Détection de présence (badge RFID ou capteur ultrason)
- Ouverture automatique
- Signalétique lumineuse de guidage
- Remontée d'état au dashboard

## Défis techniques
- Sécurité des systèmes motorisés (anti-pincement)
- Fiabilité de la détection
- Normes d'accessibilité ERP

## Technologies clés
- Arduino/ESP32, servomoteurs/vérin, RFID RC522, HC-SR04
- LED de signalisation, buzzer
- MQTT

## Ancrage Martinique
- Mise en conformité PMR des établissements antillais
- Bâtiments souvent sur plusieurs niveaux en terrain pentu
- Climat chaud : portes souvent ouvertes, gestion du flux d'air

## Interconnexions MQTT
- **Publie :** `campus/pmr/etat_porte`, `campus/pmr/detection`, `campus/pmr/alertes`
- **Consomme :** aucun

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
