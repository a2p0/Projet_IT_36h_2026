# Projet IT Première STI2D — Martinique 2025-2026

> Projet pluritechnologique collaboratif de 36 heures pour élèves de Première STI2D

[![Licence](https://img.shields.io/badge/Licence-CC--BY--SA--4.0-blue)](LICENSE)
[![Code License](https://img.shields.io/badge/Code-MIT-green)](LICENSE)
[![STI2D](https://img.shields.io/badge/STI2D-Premi%C3%A8re-orange)](https://eduscol.education.fr/)

---

## 📋 Vue d'ensemble

Ce repository contient la conception complète d'un **projet IT de fin de Première STI2D** (Innovation Technologique), conforme aux exigences officielles du BOEN et aux ressources Eduscol.

**Caractéristiques :**
- 🕐 **Durée** : 36 heures encadrées de conception-réalisation
- 👥 **Organisation** : 32 élèves, 8 groupes de 4
- 📍 **Contexte** : Lycée en Martinique (ancrage local : climat tropical, agriculture, énergie insulaire)
- 🎯 **Objectif** : Projet pluritechnologique collaboratif (approche Matière-Énergie-Information)

---

## 🎓 Référentiel officiel

- **Programme IT** : BOEN spécial n° 1 du 22 janvier 2019
- **Épreuve de contrôle continu** : BOEN n° 17 du 25 avril 2019
- **Ressource Eduscol** : Projet de fin de première STI2D (Juin 2019)

---

## 🗂️ Structure du projet

```
Projet_36h/
├── CLAUDE.md                      # Hub central du projet
├── GUIDE-CLAUDE-CLI.md            # Guide d'utilisation de Claude CLI
├── README.md                      # Ce fichier
│
├── contexte/                      # Cadre de référence stable
│   ├── cadrage-pedagogique.md    # Compétences, 6 phases Eduscol, pédagogie
│   ├── martinique.md             # Contexte local (climat, agriculture, énergie)
│   └── materiel-labo.md          # Inventaire matériel disponible
│
├── ressources/                    # Templates et références
│   ├── template-cahier-des-charges.md    # Template CDC conforme Eduscol
│   ├── competences-evaluation.md         # 7 compétences évaluées à l'oral
│   └── conventions-mqtt.md               # Protocole communication IoT
│
├── planification/                 # Suivi de projet
│   ├── calendrier.md             # Planning 36h (6 phases + 6 jalons)
│   ├── decisions.md              # Journal des décisions importantes
│   ├── questions-en-cours.md     # Points à clarifier
│   └── taches.md                 # Liste des tâches
│
├── notes/                         # Réflexions et retours
│   ├── reflexions.md
│   ├── retours-collegues.md
│   ├── ameliorations.md
│   └── mise-a-jour-eduscol-*.md  # Historique des mises à jour
│
├── theme-agricole/                # Thème 1 : Système Agricole Intelligent
│   ├── README.md                 # Scénario fédérateur, 8 sous-projets
│   ├── sous-projets/             # 8 fichiers SPn-*.md
│   ├── cahiers-des-charges/      # CDC détaillés (à rédiger)
│   └── supports-eleves/          # Fiches élèves, tutoriels
│
├── theme-batiment/                # Thème 2 : Bâtiment Scolaire Nouvelle Génération
│   ├── README.md                 # Scénario fédérateur, 8 sous-projets
│   ├── sous-projets/             # 8 fichiers SPn-*.md
│   ├── cahiers-des-charges/      # CDC détaillés (à rédiger)
│   └── supports-eleves/          # Fiches élèves, tutoriels
│
├── sources/                       # Documents sources officiels
│   └── eduscol/                  # Ressources Eduscol (PDF)
│
└── livrables/                     # Productions finales
```

---

## 🌟 Thèmes proposés

### 🌱 Thème 1 : Système Agricole Intelligent

**Scénario** : Exploitation maraîchère pilote de 2000 m² dans le sud de la Martinique (Vauclin) souhaitant devenir une vitrine de l'agriculture connectée et durable.

**8 sous-projets** :
1. SP1 - Station agro-météo
2. SP2 - Irrigation intelligente
3. SP3 - Serre bioclimatique
4. SP4 - Gestion de l'eau
5. SP5 - Centrale solaire
6. SP6 - Robot agricole
7. SP7 - Anti-nuisibles
8. SP8 - Dashboard central

**Architecture** : Noyau commun (broker MQTT + dashboard Node-RED) + modules indépendants

---

### 🏢 Thème 2 : Bâtiment Scolaire Nouvelle Génération

**Scénario** : Campus intelligent et inclusif - amélioration du cadre de vie d'un bâtiment réel du lycée.

**8 sous-projets** :
1. SP1 - Accessibilité PMR
2. SP2 - Fontaines à eau
3. SP3 - Distributeur connecté
4. SP4 - Espace détente
5. SP5 - Recharge solaire
6. SP6 - Ombrières dynamiques
7. SP7 - Micro-centrale solaire
8. SP8 - Supervision centrale

**Architecture** : Noyau commun (broker MQTT + dashboard Node-RED) + modules indépendants

---

## 🎯 Les 6 phases officielles Eduscol

| Phase | Durée | Livrables clés |
|-------|-------|----------------|
| **1. Analyse du besoin** | 3h | CDC + 5 diagrammes SysML |
| **2. Recherche d'idées** | 5h | Concept + planning Gantt + répartition tâches |
| **3. Conception détaillée** | 8h | CAO + simulations + liste composants |
| **4. Prototypage** | 14h | Prototype fonctionnel + protocole tests |
| **5. Tests et validation** | 4h | Mesures + analyse écarts + améliorations |
| **6. Restitution** | 2h | Présentation orale (20 min : 10 + 10) |

**Total** : 36 heures

---

## 📊 Évaluation

### Épreuve orale de contrôle continu (20 min)

- **10 min** : Présentation par l'élève de son travail personnel (support numérique)
- **10 min** : Dialogue argumenté avec l'interrogateur

### 7 compétences évaluées

1. **C1** - Décoder le cahier des charges
2. **C2** - Évaluer la compétitivité technique et économique
3. **C3** - Décrire avec outils de représentation adaptés (SysML, CAO, Gantt)
4. **C5** - Identifier problème technique (approche MEI)
5. **C6** - Planifier un projet (Gantt, chemin critique)
6. **C7** - Proposer des solutions (créativité, justification)
7. **C10** - Réaliser et valider prototype/maquette

**Notation** : Sur 20 points (fiche d'évaluation Banque Nationale de Sujets)

---

## 🛠️ Technologies utilisées

- **IoT** : ESP32, Arduino, capteurs (température, humidité, luminosité, etc.)
- **Communication** : MQTT (Mosquitto broker sur Raspberry Pi)
- **Dashboard** : Node-RED
- **CAO/Modélisation** : Fusion 360, SolidWorks, Papyrus SysML
- **Planification** : Diagrammes de Gantt, PERT
- **Fabrication** : Impression 3D, découpe laser, assemblage

---

## 📚 Ressources

- **Eduscol** : [STI2D - Innovation Technologique](https://eduscol.education.fr/)
- **Référentiel** : BOEN spécial n° 1 du 22 janvier 2019
- **Épreuve** : BOEN n° 17 du 25 avril 2019
- **RNR STI** : Exemples de projets IT

---

## 🚀 Comment utiliser ce repository

### Pour les enseignants

1. **Consulter `CLAUDE.md`** pour une vue d'ensemble du projet
2. **Choisir un thème** (agricole ou bâtiment) - voir `theme-*/README.md`
3. **Rédiger les CDC** en utilisant `ressources/template-cahier-des-charges.md`
4. **Suivre le planning** dans `planification/calendrier.md`
5. **Préparer l'évaluation** avec `ressources/competences-evaluation.md`

### Avec Claude CLI (IA)

Ce projet est optimisé pour être utilisé avec **Claude CLI** :
- Consultez `GUIDE-CLAUDE-CLI.md` pour 8 scénarios d'utilisation détaillés
- Contexte automatique via `CLAUDE.md`
- Templates conformes Eduscol

**Installation Claude CLI** :
```bash
npm install -g @anthropic-ai/claude-code
claude
```

---

## 📝 État d'avancement

### ✅ Fait
- [x] Cadrage pédagogique conforme Eduscol (6 phases, compétences)
- [x] Planification détaillée des 36h
- [x] Template CDC conforme fiche Eduscol (5 diagrammes SysML)
- [x] Document compétences évaluées (épreuve orale)
- [x] Identification des 8 sous-projets pour 2 thèmes
- [x] Conventions MQTT
- [x] Inventaire matériel labo

### 🔄 En cours
- [ ] Choix du thème retenu (agricole ou bâtiment)

### 📅 À venir
- [ ] Rédaction des 8 cahiers des charges détaillés
- [ ] Création des 5 diagrammes SysML par sous-projet
- [ ] Planning détaillé des 18 séances (2h × 18)
- [ ] Fiches élèves avec grille d'évaluation
- [ ] Supports ETLV (sections en anglais)

---

## 🤝 Contribution

Ce projet est partagé à des fins éducatives. Les enseignants STI2D sont invités à :
- Forker le repository
- Adapter les sous-projets à leur contexte local
- Partager leurs améliorations (pull requests)
- Signaler des problèmes ou suggestions (issues)

---

## 📄 Licence

Ce projet éducatif est sous licence **Creative Commons BY-SA 4.0** :
- ✅ Libre de partager et adapter
- ✅ Attribution requise
- ✅ Partage dans les mêmes conditions

**Attribution** : Projet IT STI2D Martinique 2025-2026

---

## 📧 Contact

Pour toute question ou suggestion : [via GitHub Issues](../../issues)

---

## 🙏 Remerciements

- Ministère de l'Éducation Nationale (ressources Eduscol)
- Communauté enseignants STI2D
- RNR STI (Réseau National de Ressources)

---

**Bonne chance pour vos projets IT !** 🚀
