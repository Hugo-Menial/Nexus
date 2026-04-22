import os

# Contenu du README au format Markdown avec optimisations visuelles GitHub
md_content = """# 🛡️ NEXUS-SQL V2.0
> **Framework Avancé de Cartographie SPA & Audit de Robustesse différentielle.**

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)
![Python Version](https://img.shields.io/badge/python-3.14-green.svg)
![Engine](https://img.shields.io/badge/engine-Async_HTTPX-orange.svg)
![Security](https://img.shields.io/badge/audit-WAF_Bypass-red.svg)

---

## 📖 Présentation
**NexusSQL** est un outil de diagnostic de sécurité conçu pour les architectures modernes (Single Page Applications). Contrairement aux outils traditionnels, il se concentre sur l'**analyse différentielle** : il mesure comment un serveur réagit à des mutations complexes pour identifier des failles logiques ou des faiblesses de filtrage.

---

## 🚀 Fonctionnalités Clés

### 🔍 1. SPA Deep Discovery
Utilise **Playwright** pour simuler une navigation humaine, capturer les appels API asynchrones et cartographier les endpoints JSON souvent invisibles pour les scanners classiques.

### 🎭 2. Moteur de Mutation Polymorphique
Le `StringMutator` génère des variantes de payloads capables de contourner les WAF (Web Application Firewalls) :
* **Double Encodage URL** (`%2527`)
* **Fragmentation SQL** (Insertion de commentaires `/**/` stratégiques)
* **Polymorphisme de Casse** (Altération majuscule/minuscule intelligente)

### 🕵️ 3. Fuzzing Furtif (Stealth)
* **Jitter Adaptatif** : Distribution de Poisson pour espacer les requêtes et éviter le bannissement IP.
* **Session Persistence** : Import de cookies JSON pour auditer les zones authentifiées.
* **Fingerprint Mimicry** : Simulation de headers de navigateurs modernes (Chrome 124+).

### 📊 4. Dashboard de Conformité
Interface **Streamlit** offrant :
* Un résumé visuel de la résilience du site.
* Une matrice détaillée de chaque test effectué.
* Un export des données pour les rapports d'audit.

---

## 🛠️ Installation & Utilisation

### Installation
```bash
git clone [https://github.com/votre-repo/nexus-sql.git](https://github.com/votre-repo/nexus-sql.git)
cd nexus-sql
pip install -r requirements.txt
playwright install
