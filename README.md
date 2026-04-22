# 🛡️ NEXUS-SQL 
> **Framework de Diagnostic de Robustesse pour Single Page Applications (SPA)**

NexusSQL est une solution d'audit de sécurité automatisée conçue pour cartographier les API modernes et tester leur résilience face à des mutations de payloads avancées. Il combine l'exploration dynamique par navigateur et l'analyse différentielle de trafic.

---

## 📊 Aperçu du Framework
NexusSQL n'est pas un simple scanner de vulnérabilités. C'est un outil de **QA Sécurité** qui vérifie la solidité des filtres applicatifs via :
- **Discovery** : Cartographie des endpoints via Playwright.
- **Mutation** : Polymorphisme de payloads (Double encoding, Fragmentation SQL).
- **Stealth** : Simulation de comportement humain (Jitter, Cookies, Fingerprinting).
- **Reporting** : Dashboard de conformité temps-réel avec Streamlit.

---

## 🛠️ Architecture du Projet

Le projet est structuré en 4 modules interdépendants :

| Fichier | Rôle |
| :--- | :--- |
| `spa_mapper.py` | Crawling dynamique et extraction des routes d'API JSON. |
| `string_mutator.py` | Moteur de polymorphisme (génération des variantes de payloads). |
| `robustness_engine.py` | Moteur d'audit asynchrone (gestion du Jitter et des sessions). |
| `dashboard.py` | Interface de visualisation et rapport de conformité. |

---

## ⚙️ Installation

### 1. Prérequis
* Python 3.14+
* Google Chrome (pour Playwright)

### 2. Configuration de l'environnement
```powershell
# Cloner le projet
git clone [https://github.com/votre-repo/testi.git](https://github.com/votre-repo/testi.git)
cd testi

# Installer les dépendances
pip install httpx playwright streamlit pandas

# Initialiser le moteur de rendu
playwright install chromium
