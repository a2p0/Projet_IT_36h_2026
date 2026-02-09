# Thème 1 — Système Agricole Intelligent

## Scénario fédérateur

Une exploitation maraîchère pilote de 2000 m² dans le sud de la Martinique (plaine du Vauclin) souhaite devenir une vitrine de l'agriculture connectée et durable. Elle cultive des légumes pays (dachines, patates douces, piments, giraumons) et du maraîchage classique (tomates, salades, concombres).

L'exploitant souhaite moderniser sa ferme en intégrant des technologies IoT, des énergies renouvelables et de l'automatisation, tout en respectant une démarche zéro-phyto et en optimisant sa consommation d'eau.

## Noyau commun

Tous les modules communiquent via un **broker MQTT commun** hébergé sur un Raspberry Pi central (géré par le SP8). Chaque groupe publie ses données sur des topics MQTT normalisés et peut s'abonner aux données des autres groupes.

### Protocole de communication partagé

- **Broker :** Mosquitto sur Raspberry Pi
- **Format des messages :** JSON avec structure normalisée
- **Convention de topics :** `ferme/{module}/{type_donnee}` (ex: `ferme/meteo/temperature`)
- **Dashboard :** Interface web Node-RED accessible à tous les groupes

### Livrable collectif initial

En début de projet, les 8 groupes définissent ensemble :
- La convention de nommage des topics MQTT
- Le format JSON des messages (clés, unités, horodatage)
- Les données que chaque module publie et consomme

## Vue d'ensemble des 8 sous-projets

| SP | Nom | Dominante MEI | Interconnexions |
|----|-----|---------------|-----------------|
| SP1 | Station agro-météo | Information > Énergie > Matière | Fournit données à SP2, SP3, SP6, SP7 |
| SP2 | Irrigation intelligente | Information > Matière > Énergie | Consomme SP1 (météo), SP4 (eau), SP5 (énergie) |
| SP3 | Serre bioclimatique | Matière > Information > Énergie | Consomme SP1 (météo) |
| SP4 | Gestion de l'eau | Matière > Énergie > Information | Fournit données à SP2 |
| SP5 | Centrale solaire | Énergie > Information > Matière | Fournit énergie à tous |
| SP6 | Robot agricole | Matière > Énergie > Information | Consomme SP1 (météo) |
| SP7 | Anti-nuisibles | Information > Matière > Énergie | Consomme SP1 (météo) |
| SP8 | Dashboard central | Information > Matière > Énergie | Agrège toutes les données |

## Statut

- [x] Identification des sous-projets
- [ ] Cahiers des charges détaillés
- [ ] Modélisation SysML
- [ ] Planning des 36h
