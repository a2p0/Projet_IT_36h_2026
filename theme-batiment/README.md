# Thème 2 — Bâtiment Scolaire Nouvelle Génération

## Scénario fédérateur

Le lycée engage une démarche « campus intelligent et inclusif » pour améliorer le cadre de vie des élèves et des personnels. Un bâtiment réel de l'établissement sert de base d'étude. Chaque groupe conçoit un module d'amélioration alliant développement durable et services concrets.

Les irritants identifiés dans le quotidien du lycée : accessibilité PMR insuffisante, manque de fontaines à eau, absence de distributeurs connectés, pas d'espace détente aménagé, pas de points de recharge, zones d'ombre insuffisantes dans la cour, dépendance au réseau électrique classique.

## Noyau commun

Comme pour le thème agricole, tous les modules communiquent via un **broker MQTT commun** sur Raspberry Pi et alimentent un **tableau de bord de supervision** du campus.

### Protocole de communication partagé

- **Broker :** Mosquitto sur Raspberry Pi
- **Format des messages :** JSON normalisé
- **Convention de topics :** `campus/{module}/{type_donnee}` (ex: `campus/fontaine/temperature_eau`)
- **Dashboard :** Interface web Node-RED

### Livrable collectif initial

Définition commune des conventions MQTT (topics, format JSON, unités).

## Vue d'ensemble des 8 sous-projets

| SP | Nom | Dominante MEI | Interconnexions |
|----|-----|---------------|-----------------|
| SP1 | Accessibilité PMR | Matière > Information > Énergie | Publie état portes/rampes |
| SP2 | Fontaines à eau | Matière > Énergie > Information | Consomme SP7 (énergie) |
| SP3 | Distributeur connecté | Matière > Information > Énergie | Consomme SP7 (énergie) |
| SP4 | Espace détente | Information > Matière > Énergie | Publie fréquentation |
| SP5 | Recharge solaire | Énergie > Information > Matière | Fournit énergie locale |
| SP6 | Ombrières dynamiques | Matière > Énergie > Information | Consomme données météo |
| SP7 | Micro-centrale solaire | Énergie > Information > Matière | Fournit énergie à tous |
| SP8 | Supervision centrale | Information > Matière > Énergie | Agrège tout |

## Statut

- [x] Identification des sous-projets
- [ ] Cahiers des charges détaillés
- [ ] Modélisation SysML
- [ ] Planning des 36h
