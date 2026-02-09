# Conventions MQTT — Référence technique

## Architecture

```
[ESP32/Arduino] --WiFi--> [Broker Mosquitto (Raspberry Pi)] <--WiFi-- [Dashboard Node-RED]
     Module 1-7                      SP8                              SP8
```

## Convention de topics

### Thème agricole
```
ferme/{module}/{type_donnee}
```

Exemples :
- `ferme/meteo/temperature`
- `ferme/irrigation/humidite_sol`
- `ferme/energie/production`
- `ferme/systeme/alertes`

### Thème bâtiment
```
campus/{module}/{type_donnee}
```

Exemples :
- `campus/fontaine/temperature_eau`
- `campus/energie/production`
- `campus/systeme/etat`

## Format JSON normalisé

Chaque message MQTT doit respecter cette structure :

```json
{
  "module": "meteo",
  "capteur": "temperature",
  "valeur": 28.5,
  "unite": "°C",
  "timestamp": 1700000000,
  "qualite": "ok"
}
```

### Champs obligatoires
- `module` : identifiant du sous-projet émetteur
- `capteur` : type de mesure
- `valeur` : donnée numérique ou texte
- `unite` : unité de mesure (chaîne vide si sans unité)

### Champs optionnels
- `timestamp` : horodatage Unix (secondes)
- `qualite` : `"ok"`, `"degradee"`, `"erreur"`
- `seuil_bas`, `seuil_haut` : pour les alertes

## QoS recommandé

- **QoS 0 (at most once)** : données de capteurs régulières (température, humidité)
- **QoS 1 (at least once)** : alertes et événements importants

## Fréquence de publication

- Données capteurs : toutes les 10-30 secondes
- Alertes : immédiat
- États système : toutes les 60 secondes

## Bibliothèques recommandées

- **ESP32/Arduino :** PubSubClient (`#include <PubSubClient.h>`)
- **Raspberry Pi (Python) :** paho-mqtt (`import paho.mqtt.client as mqtt`)
- **Node-RED :** nœuds MQTT intégrés
