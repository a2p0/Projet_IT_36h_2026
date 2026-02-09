# SP5 — Centrale solaire de l'exploitation

> Dimensionner et piloter la production d'énergie renouvelable pour l'ensemble du site.

## Déclinaison MEI

### Matière
- Support orientable pour panneau solaire (maquette)
- Étude de l'inclinaison optimale à la latitude de la Martinique (14.6°N)
- Matériaux résistants à la corrosion (inox, aluminium)

### Énergie
- Dimensionnement de l'installation (bilan de puissance de tous les modules)
- Régulateur de charge, stockage batterie
- Distribution vers les autres sous-projets

### Information
- Monitoring de production (courant, tension, puissance)
- Suivi du rendement et de l'état de charge batterie
- Dashboard énergétique dédié

## Défis techniques
- Bilan de puissance réaliste intégrant tous les SP
- Gestion de l'intermittence (passages nuageux tropicaux)
- Protection contre les surtensions

## Technologies clés
- Panneau solaire 20-50W, régulateur de charge PWM/MPPT
- Batterie plomb ou Li-ion, capteurs INA219 (courant/tension)
- ESP32, MQTT

## Ancrage Martinique
- Ensoleillement exceptionnel (~5 kWh/m²/jour)
- Coût élevé de l'électricité en Martinique
- Objectif d'autonomie énergétique insulaire

## Interconnexions MQTT
- **Publie :** `ferme/energie/production`, `ferme/energie/batterie`, `ferme/energie/consommation`
- **Consomme :** `ferme/meteo/uv` (SP1, pour corrélation production/ensoleillement)

## Statut
- [ ] Cahier des charges
- [ ] Modélisation SysML
- [ ] Prototype
