# CV Web — Gabriel VIDEIRA · Head of SEO/GEO Groupe

Page web responsive du CV Axe 2 (disruptif "Auto-SEO/GEO") — candidature Magnolia.

🔗 **Live:** *à mettre à jour après déploiement GitHub Pages*

## Concept

Cette page n'est pas un CV qui parle de SEO/GEO. **C'est un CV qui *est* une démonstration vivante de SEO/GEO.**

Le rendu visuel imite une réponse IA générée (style Perplexity / Google AI Overview) — barre de recherche, AI Overview block avec citations [1] [2] [3] cliquables, panel "People Also Ask" interactif, schema markup JSON-LD visible.

Mais ce n'est pas qu'esthétique : la page intègre vraiment :
- ✅ **JSON-LD Schema.org** (`Person` + `FAQPage`) directement dans le `<head>`
- ✅ **Meta tags** OpenGraph + description optimisés pour citation LLM
- ✅ **`llms.txt`** racine du site pour guider les crawlers IA
- ✅ Structure HTML sémantique avec headings hiérarchiques
- ✅ Citations courtes et factuelles (chunks digestibles par les LLMs)
- ✅ FAQ format question-réponse (favorisé par AI Overviews)

→ Cette page est conçue pour être **citée** par ChatGPT, Perplexity, Gemini, Claude et les AI Overviews Google.

## Features

- 🌓 Mode dark / light avec persistance localStorage
- ⌨️ Animation typewriter sur la barre de recherche
- 🔗 Citations cliquables qui scrollent vers la source correspondante
- ❓ People Also Ask repliables au clic
- 📱 Full responsive (mobile-first)
- ⚡ Single-file HTML (~100 KB avec photo en base64) — chargement instantané

## Déploiement GitHub Pages — 3 étapes

### 1. Créer un repo GitHub

```bash
# Sur GitHub → New repository → nom suggéré : cv-magnolia (ou ce que tu veux)
# Public, pas de README/gitignore (on a déjà tout)
```

### 2. Pousser les fichiers

```bash
cd /chemin/vers/dossier/contenant/index.html
git init
git add index.html llms.txt README.md
git commit -m "feat: CV Head of SEO Magnolia — initial deploy"
git branch -M main
git remote add origin https://github.com/TON_USER/cv-magnolia.git
git push -u origin main
```

### 3. Activer GitHub Pages

- Aller dans le repo → **Settings** → **Pages** (menu de gauche)
- Source: **Deploy from a branch**
- Branch: **main** / Folder: **/ (root)** → **Save**
- Attendre ~1-2 minutes
- L'URL sera : `https://TON_USER.github.io/cv-magnolia/`

### Bonus — domaine personnalisé (optionnel)

Si tu as un domaine, tu peux le pointer sur GitHub Pages :
- Créer un fichier `CNAME` à la racine du repo contenant : `cv.gabriel-videira.com`
- Config DNS : ajouter un enregistrement CNAME pointant vers `TON_USER.github.io`

## Fichiers

| Fichier | Description |
|---------|-------------|
| `index.html` | La page complète (HTML+CSS+JS+photo base64) |
| `llms.txt` | Guide pour les crawlers IA (optimisation GEO) |
| `README.md` | Ce fichier |

## Tech stack

- Pure HTML/CSS/JavaScript (aucune dépendance, aucun build)
- Photo embarquée en base64 (autonomie totale)
- Schema.org JSON-LD (Person + FAQPage)
- Compatible tous navigateurs modernes
- Score Lighthouse Performance/SEO/Accessibility visé : 95+

## Crédits

Conçu par Gabriel VIDEIRA pour la candidature Head of SEO Groupe @ Groupe Magnolia · Avril 2026.
