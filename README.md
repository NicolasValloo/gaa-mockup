# GAA — Maquette interactive

Maquette HTML/CSS/JS du logiciel **GAA (Gestion d'Agence d'Architecture)** — 16 écrans couvrant l'ensemble des modules fonctionnels.

## Structure

```
gaa-app/
├── index.html          ← Point d'entrée (shell navigation + iframe)
├── dashboard.html      ← 📊 Tableau de bord dirigeant
├── projets.html        ← 📁 Portefeuille projets
├── fiche-projet.html   ← 📋 Fiche projet détaillée + phases MOP
├── temps.html          ← ⏱️ Saisie des temps / pointage
├── finances.html       ← 💰 Finances & facturation
├── contacts.html       ← 👥 CRM & contacts
├── taches.html         ← ✅ Gestion des tâches (Kanban/liste/calendrier)
├── parametrage.html    ← ⚙️ Administration & paramétrage
├── planning.html       ← 📅 Planning de charge (heatmap/Gantt)
├── documents.html      ← 📄 GED — Gestion documentaire
├── chantier.html       ← 🏗️ Suivi de chantier (CR/réserves/VISA)
├── reporting.html      ← 📈 Reporting & Business Intelligence
├── alertes.html        ← 🔔 Alertes & Automatisation (workflows)
├── messagerie.html     ← 💬 Messagerie & Base de connaissances
├── assurances.html     ← 🛡️ Assurances & Intégrations
├── portail.html        ← 🌐 Portail externe MOA/BET/Entreprises
└── README.md
```

## Mise en ligne avec GitHub Pages

### 1. Créer le dépôt

```bash
# Créer un nouveau dépôt sur github.com (ex: gaa-mockup)
# Puis localement :
cd gaa-app
git init
git add .
git commit -m "GAA - Maquette interactive complète (16 écrans)"
git branch -M main
git remote add origin https://github.com/VOTRE-USERNAME/gaa-mockup.git
git push -u origin main
```

### 2. Activer GitHub Pages

1. Aller sur **github.com/VOTRE-USERNAME/gaa-mockup**
2. **Settings** → **Pages** (menu gauche)
3. **Source** : sélectionner **Deploy from a branch**
4. **Branch** : `main` / `/ (root)`
5. Cliquer **Save**

### 3. Accéder au site

Après 1-2 minutes, le site est disponible à :

```
https://VOTRE-USERNAME.github.io/gaa-mockup/
```

### Alternative : Netlify (plus rapide)

1. Aller sur [app.netlify.com](https://app.netlify.com)
2. Drag & drop le dossier `gaa-app/` sur la page
3. Le site est en ligne immédiatement avec une URL type `random-name.netlify.app`
4. Possibilité de configurer un domaine personnalisé

### Alternative : Vercel

```bash
npm i -g vercel
cd gaa-app
vercel
```

## Caractéristiques techniques

- **Aucune dépendance** — HTML/CSS/JS pur, pas de build
- **747 Ko** total — chargement instantané
- **Navigation par iframe** — le shell (index.html) charge chaque écran
- **Raccourcis clavier** — Alt+1 à Alt+0 pour naviguer
- **Responsive** — Desktop / Tablette / Mobile
- **Charte graphique** — Inter + JetBrains Mono, palette WCAG AA

## Modules couverts

| # | Écran | Modules spec |
|---|---|---|
| 1 | Tableau de bord | 2.2 |
| 2 | Portefeuille projets | 1.1 |
| 3 | Fiche projet | 1.1, 1.2 |
| 4 | Saisie des temps | 1.3 |
| 5 | Finances & facturation | 1.5 |
| 6 | CRM & contacts | 1.6 |
| 7 | Gestion des tâches | 1.9 |
| 8 | Paramétrage | 2.1, 2.3, 2.4, 2.5, 2.6 |
| 9 | Planning de charge | 1.7 |
| 10 | Gestion documentaire | 1.4 |
| 11 | Suivi de chantier | 1.8 |
| 12 | Reporting & BI | 4.1 |
| 13 | Alertes & workflows | 4.2, 4.3 |
| 14 | Messagerie & connaissances | 4.4, 4.6 |
| 15 | Assurances & intégrations | 1.10, 3.1→3.5 |
| 16 | Portail externe | 4.5 |
