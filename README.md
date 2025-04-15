# Projet Black-Litterman

Ce dossier contient un projet Quarto complet pour la génération automatique d'un rapport PDF ou HTML à partir d’un notebook Jupyter.

## 📁 Structure du dossier

| Fichier / Dossier               | Description                                                  |
| ------------------------------- | ------------------------------------------------------------ |
| `Projet_Black-Litterman.ipynb`  | Le notebook principal contenant le contenu du rapport (texte + code Python). |
| `Projet_Black-Litterman.qmd`    | Version convertie du notebook en Quarto Markdown (optionnel, utilisé si vous éditez sans Jupyter). |
| `_quarto.yml`                   | Fichier de configuration global définissant le style PDF/HTML (marges, police, en-têtes, etc.). |
| `Projet_Black-Litterman.pdf`    | Rapport PDF généré avec table des matières, style personnalisé, etc. |
| `Projet_Black-Litterman.html`   | Version HTML interactive du rapport.                         |
| `Projet_Black-Litterman_files/` | Dossier généré automatiquement pour les ressources associées à l’HTML. |
| `readme.md`                     | Ce fichier d’explication du projet.                          |

## ⚙️ Comment utiliser ce projet

### 1. Prérequis

Assurez-vous que vous avez installé :

- [Quarto](https://quarto.org/)
- Python (avec `jupyter`, `pandas`, `numpy`, etc.)
- Un moteur LaTeX (`TinyTeX`, `MacTeX`, `TeX Live`...)

Installez les dépendances Python si besoin :

```bash
pip install jupyter numpy pandas matplotlib etc.
```

### 2. Pour générer le PDF ou HTML

Placez-vous dans le dossier du projet puis exécutez :

```bash
quarto render Projet_Black-Litterman.ipynb --to pdf
# ou
quarto render Projet_Black-Litterman.ipynb --to html
# ou simplement
quarto render 
```

