# 🧠 Crack the Code — V6

**Neurosciences appliquées à la réduction des risques.**  
Protocoles validés · Données locales · 100% gratuit · Sans pub · Sans collecte de données.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Live Demo](https://img.shields.io/badge/Demo-GitHub%20Pages-brightgreen)](https://podarcis-cloud.github.io/Crack-the-code-v6/)
[![PWA Ready](https://img.shields.io/badge/PWA-Installable-purple)](https://podarcis-cloud.github.io/Crack-the-code-v6/)
[![Langues](https://img.shields.io/badge/Langue-Français-red)](https://podarcis-cloud.github.io/Crack-the-code-v6/)

-----

## 🌐 Demo live

**<https://podarcis-cloud.github.io/Crack-the-code-v6/>**

Installable sur mobile : Safari → *Partager → Sur l’écran d’accueil* · Chrome → *Installer l’application*

-----

## 📋 À propos

Crack the Code V6 est une application web progressive (PWA) de **réduction des risques liés aux substances psychoactives**, construite entièrement en HTML/CSS/JS vanilla. Elle ne requiert aucun serveur, aucune base de données, aucune inscription.

> ⚠️ **Information préventive** — Ces outils s’adressent aux personnes qui consomment déjà. Ils ne remplacent pas un suivi médical. En cas d’urgence : **112** (BE/CH/LU) · **15** (FR) · **911** (CA)

-----

## 🗂 Modules

|Module               |Fichier                  |Description                                                                 |Taille|
|---------------------|-------------------------|----------------------------------------------------------------------------|------|
|🏠 Cockpit            |`index.html`             |Login, session, navigation vers tous les modules                            |13 Ko |
|🧩 Tetris Anti-Craving|`tetris.html`            |Interférence visuospatiale Oxford 2015 — 3 min réduisent le craving de 24%  |17 Ko |
|🌀 Gyro Labyrinthe    |`maze.html`              |Gyroscope / flèches tactiles · 3 niveaux · Cervelet & Vestibulaire          |22 Ko |
|🔬 PSYCHOchecker      |`psychochecker.html`     |172 substances · 150+ interactions · Cannabinoïdes · Tri alphabétique       |102 Ko|
|📋 Exercices & Bilans |`fiches.html`            |20 exercices neuroscience · 3 questionnaires validés (AUDIT, Craving, WHO-5)|30 Ko |
|🤖 RDR & Dr. Alex IA  |`rdr.html`               |Urgences · Centres par région · Agent IA addictologue (Groq)                |32 Ko |
|📊 Journal de Suivi   |`suivi.html`             |Calendrier 30j · Streak · Coûts · Test salivaire scientifique               |52 Ko |
|🧬 Profil Neurologique|`profil.html`            |DAST-10 · AUDIT-10 · BIS-11 · GAD-7 · PHQ-9 · Radar neuro canvas            |40 Ko |
|💛 Soutenir           |`soutenir.html`          |Roadmap · Dons · Partage                                                    |20 Ko |
|⚙️ PWA                |`sw.js` + `manifest.json`|Service Worker offline + manifest installable                               |—     |
|🔧 Proxy (optionnel)  |`worker.js`              |Cloudflare Worker pour clé API alternative                                  |—     |

-----

## ✨ Fonctionnalités détaillées

### 🧩 Tetris Anti-Craving

- Protocole **Oxford 2015** (Skorka-Brown et al.) — le Tetris mobilise le cortex visuospatial, court-circuitant les images mentales du craving
- Sessions de **3 minutes** avec option de continuer (+3 min, vitesse croissante à chaque session)
- Pièce fantôme, contrôles tactiles sans double-déclenchement
- Barre craving temps réel, sauvegarde automatique des sessions

### 🌀 Gyro Labyrinthe

- 3 niveaux de difficulté progressifs
- **Gyroscope** (iOS/Android) avec fallback flèches tactiles
- Résolution de collisions précise, pénalités de temps
- Score 5/5 par niveau, historique sauvegardé

### 🔬 PSYCHOchecker RDR

- **172 substances** documentées : stimulants, dépresseurs, opioïdes, psychédéliques, cannabinoïdes, dissociatifs, designer drugs, nootropiques
- **150+ interactions** documentées avec classification :
  - 💀 Potentiellement mortelles
  - 🔴 Risque sévère
  - ⚠️ Vigilance requise
  - ✅ Non documentée / faible risque
- Vérificateur **multi-paires** (3 substances simultanées)
- **Autocomplétion** avec 172 alias (noms de rue, noms de marque, noms scientifiques)
- Liste triée alphabétiquement, filtres par famille
- Onglet cannabinoïdes synthétiques séparé (JWH, ADB, 5F-ADB, HHC-P, etc.)

### 📋 Exercices & Bilans

- **20 exercices neuroscience** validés, organisés en 3 catégories :
  - Crise / craving immédiat (Tetris Mental, Glaçon, Surf l’Envie, Respiration Carrée…)
  - Quotidien (Menu Dopamine, Lettre au Futur Toi, Gratitude Punk…)
  - Plasticité cérébrale (Stroop, Dual Task, Polymétrie, Alphabet inverse…)
- Timers interactifs avec messages de progression
- **3 questionnaires validés** : AUDIT-C Alcool · Bilan Craving · WHO-5 Bien-être
- Historique des bilans en localStorage

### 🤖 RDR & Dr. Alex IA

- **Dr. Alex** : agent IA combinant addictologue, psychologue et assistant social
- Basé sur **Groq API** (gratuit) · Modèle `llama-3.3-70b-versatile`
- Contexte personnalisé : profil neurologique + journal de suivi + âge + région
- 8 boutons de démarrage rapide
- **4 onglets** :
  - 🤖 Dr. Alex (chat IA)
  - 🚨 Urgences (numéros cliquables par région)
  - 🛡 RDR pratique (protocoles, PLS, Naloxone, post-MDMA…)
  - 📍 Centres (annuaire par région avec liens)
- Couverture : 🇧🇪 Belgique · 🇫🇷 France · 🇨🇭 Suisse · 🇨🇦 Canada QC · 🇱🇺 Luxembourg

### 📊 Journal de Suivi

- **Calendrier 30 jours** coloré par intensité (sobre/léger/modéré/intensif), cliquable
- Modal détail par jour avec liste des prises, possibilité de supprimer
- Jours vides → bouton direct vers le journal avec date pré-remplie
- **Streak de sobriété** avec record personnel
- Graphique barres 8 semaines, tendance par substance
- **Onglet Coûts** :
  - Totaux 7j / 30j / 90j / cumulé
  - Projection annuelle
  - Breakdown par substance (barres + moyenne €/prise)
  - Coût d’opportunité (que pourrais-tu faire avec cet argent ?)
- **Module test salivaire scientifique** :
  - Fenêtres en heures (min–max) par substance
  - Sources : SAMHSA/DOT 2023 · Desrosiers & Huestis (2019) J Anal Toxicol · NIH PMC2700061
  - Date exacte “test négatif probable dès le” + “usage régulier jusqu’au”
  - Autocomplétion liée aux 172 substances du PSYCHOchecker
- **Onglet Objectifs** : streak, réduction, max/semaine, aucune séance intense

### 🧬 Profil Neurologique

- **6 évaluations validées** :
  - DAST-10 (Drug Abuse Screening Test — OMS)
  - AUDIT-10 (Alcohol Use Disorders Identification Test — OMS)
  - BIS-11 adapté (Barratt Impulsiveness Scale)
  - GAD-7 adapté (Generalized Anxiety Disorder)
  - PHQ-9 adapté (Patient Health Questionnaire — dépression)
  - Stades de Prochaska & DiClemente (motivation au changement)
- **Radar neurologique** dessiné en Canvas (4 axes : contrôle inhibiteur, résistance craving, régulation émotionnelle, plasticité motivationnelle)
- Explication neurobiologique personnalisée + recommandations par niveau
- Intégré dans le contexte de Dr. Alex

-----

## 🚀 Installation

### Option 1 — GitHub Pages (déjà en ligne)

```
https://podarcis-cloud.github.io/Crack-the-code-v6/
```

### Option 2 — En local

```bash
git clone https://github.com/podarcis-cloud/Crack-the-code-v6.git
cd Crack-the-code-v6
# Ouvrir index.html dans un navigateur
# OU lancer un serveur local :
python3 -m http.server 8080
# → http://localhost:8080
```

### Option 3 — Déployer sur son propre hébergement

Copier tous les fichiers `.html`, `sw.js` et `manifest.json` dans le dossier racine de n’importe quel hébergement statique (Netlify, Vercel, Cloudflare Pages, etc.).

-----

## 🤖 Activer Dr. Alex IA (Groq — gratuit)

L’agent IA Dr. Alex utilise l’API **Groq** — 100% gratuite, aucune carte bancaire.

**En 2 minutes :**

1. Aller sur [console.groq.com](https://console.groq.com) → créer un compte gratuit
1. *API Keys* → *Create API Key* → copier la clé (`gsk_...`)
1. Dans `rdr.html`, ligne ~389, remplacer :
   
   ```javascript
   const GROQ_API_KEY = 'COLLE_TA_CLÉ_GROQ_ICI';
   ```
   
   par ta clé :
   
   ```javascript
   const GROQ_API_KEY = 'gsk_ton_vrai_token_ici';
   ```
1. Pousser sur GitHub → Dr. Alex est actif ✓

**Limites gratuites Groq :** 14 400 requêtes/jour · 6 000 tokens/min · Aucune expiration

> **Alternative payante :** Un proxy Cloudflare Worker (`worker.js` fourni) permet d’utiliser l’API Anthropic Claude. Voir <SETUP.md> pour le détail.

-----

## 📐 Architecture technique

```
crack-the-code-v6/
├── index.html          # Cockpit — session localStorage, routing
├── tetris.html         # Module Tetris
├── maze.html           # Module Labyrinthe gyroscope
├── psychochecker.html  # Base données substances + interactions
├── fiches.html         # Exercices + questionnaires
├── rdr.html            # RDR + Dr. Alex (Groq API)
├── suivi.html          # Journal + coûts + test salivaire
├── profil.html         # Évaluations + radar neuro
├── soutenir.html       # Soutien projet
├── sw.js               # Service Worker (PWA offline)
├── manifest.json       # Web App Manifest
├── worker.js           # Cloudflare Worker proxy (optionnel)
├── SETUP.md            # Guide activation IA
└── README.md
```

**Stack :** HTML5 · CSS3 vanilla · JavaScript ES6+ vanilla · localStorage · Canvas API · DeviceOrientation API · Service Worker API · Groq API (LLaMA 3.3 70B)

**Aucune dépendance externe** côté code (0 framework, 0 npm). Seule Google Fonts est chargée en CDN.

**Données :** 100% localStorage côté client. Rien n’est envoyé à un serveur (sauf les messages Dr. Alex à l’API Groq).

-----

## 🔬 Bases scientifiques

|Module             |Sources                                                                                                     |
|-------------------|------------------------------------------------------------------------------------------------------------|
|Tetris Anti-Craving|Skorka-Brown et al. (2015) *Addictive Behaviors* — Oxford University                                        |
|Test salivaire     |SAMHSA/DOT Mandatory Guidelines (2023) · Desrosiers & Huestis (2019) *J Anal Toxicol 43(6)* · NIH PMC2700061|
|DAST-10            |Harvey A. Skinner (1982) — OMS / NIDA                                                                       |
|AUDIT-10           |Saunders et al. (1993) — OMS                                                                                |
|PHQ-9              |Kroenke & Spitzer (2002)                                                                                    |
|GAD-7              |Spitzer et al. (2006)                                                                                       |
|BIS-11             |Barratt (1994) — adapté                                                                                     |
|Stades Prochaska   |Prochaska & DiClemente (1983)                                                                               |
|Exercices neuro    |Hebb (1949) · Draganski et al. (2004) · Erickson et al. (2011)                                              |
|Réduction risques  |EMCDDA Guidelines · OMS · Marlatt (1985) — Urge Surfing                                                     |

-----

## 🌍 Couverture régionale

|Région      |Urgences                                                 |Centres                                 |Conseils                          |
|------------|---------------------------------------------------------|----------------------------------------|----------------------------------|
|🇧🇪 Belgique  |112 · Anti-Poisons 070 245 245 · Drogues Info 0800 10 800|Trempoline · Modus Vivendi · Alfa · MASS|Testing · Naloxone sans ordonnance|
|🇫🇷 France    |15 · Drogues Info 0800 23 13 13 · 3114                   |CSAPA · Techno+                         |Mon Soutien Psy · Nightline       |
|🇨🇭 Suisse    |144 · Tox Info 145 · 143                                 |Fondation Phénix · ARUD · SuchtSchweiz  |Salles de consommation légales    |
|🇨🇦 Canada QC |911 · Antipoison 1-800-463-5060                          |Portage · GRIP · CRAN                   |Naloxone gratuite RAMQ            |
|🇱🇺 Luxembourg|112 · SOS Détresse 454545                                |JDH · Abrigado                          |CNS rembourse                     |

-----

## 📱 PWA — Installation mobile

**iOS (Safari) :**

1. Ouvrir le lien dans Safari
1. Icône de partage → *Sur l’écran d’accueil*
1. Nommer l’app → *Ajouter*

**Android (Chrome) :**

1. Ouvrir le lien dans Chrome
1. Menu ⋮ → *Installer l’application* ou bandeau automatique

L’application fonctionne ensuite **hors ligne** (tous les modules sauf Dr. Alex qui nécessite une connexion internet).

-----

## 🔒 Vie privée

- **Aucune donnée personnelle collectée** par le projet
- Toutes les données (journal, profil, sessions) sont stockées **uniquement en localStorage** sur l’appareil
- Les messages Dr. Alex sont envoyés à l’API **Groq** (ou Anthropic si proxy) — consulter leurs politiques de confidentialité respectives
- Aucun cookie, aucun tracking, aucune analytics

-----

## 🤝 Contribuer

Les contributions sont les bienvenues !

```bash
# Fork → Clone → Branch
git checkout -b feature/ma-fonctionnalite

# Tester en local
python3 -m http.server 8080

# Pull Request → main
```

**Idées de contributions :**

- Nouvelles substances ou interactions documentées (avec sources)
- Traductions (EN · NL · DE · ES · PT)
- Nouveaux exercices neuroscience (avec références)
- Amélioration de l’accessibilité (WCAG)
- Tests automatisés
- Mode sombre (actuellement bloqué volontairement pour lisibilité)

**Guidelines :**

- Citer les sources scientifiques pour toute donnée médicale ou pharmacologique
- Respecter l’approche sans jugement et centrée sur la réduction des risques
- Ne pas ajouter de dépendances npm côté client

-----

## 📝 Changelog

### V6 (actuelle)

- ✅ Agent IA Dr. Alex (addictologue · psychologue · assistant social) via Groq
- ✅ Journal de suivi avec calendrier coloré cliquable
- ✅ Onglet Coûts avec projection annuelle et coût d’opportunité
- ✅ Test salivaire scientifique (fenêtres en heures, sources SAMHSA/Desrosiers 2019)
- ✅ Profil neurologique avec 6 évaluations validées et radar Canvas
- ✅ 172 substances + 150+ interactions dans PSYCHOchecker
- ✅ Tetris avec sessions continues (vitesse progressive)
- ✅ Labyrinthe gyroscope 3 niveaux
- ✅ PWA installable avec Service Worker offline
- ✅ Dark mode bloqué (lisibilité garantie)
- ✅ Autocomplétion substances liée au PSYCHOchecker

### V5

- Base PSYCHOchecker
- Modules Tetris et Labyrinthe (versions préliminaires)
- Page RDR statique

-----

## ⚖️ Licence

MIT — voir <LICENSE>

-----

## 💛 Soutenir le projet

Crack the Code est gratuit, sans pub et sans collecte de données. Si tu trouves ce projet utile :

- ⭐ **Star** ce repository
- 📲 **Partager** l’application à quelqu’un qui pourrait en avoir besoin
- 💬 **Ouvrir une issue** pour signaler un bug ou proposer une amélioration
- 💶 **Don** via la page [Soutenir](https://podarcis-cloud.github.io/Crack-the-code-v6/soutenir.html)

-----

## ⚠️ Avertissement

> Cette application fournit des informations à but **éducatif et préventif**. Elle ne remplace en aucun cas un avis médical, une consultation psychiatrique ou un suivi addictologique professionnel.  
> En cas d’urgence médicale, appelez le **112** (BE/CH/LU), le **15** (FR) ou le **911** (CA).  
> En cas de pensées suicidaires : **3114** (FR) · **0800 32 123** (BE) · **143** (CH) · **1 866 APPELLE** (CA)

-----

<div align="center">
  <sub>Fait avec 🧠 pour les personnes qui font des choix éclairés · Belgique · 2025</sub>
</div>