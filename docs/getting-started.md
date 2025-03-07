# Prise en main de LazyGit

---

## Premier lancement

```bash
# Lancement simple
lazygit

# Avec alias (recommandé)
lg
```

---

## Interface principale

| Zone | Description |
|------|-------------|
| **Status** | État des fichiers et du dépôt |
| **Files** | Liste des fichiers modifiés |
| **Branches** | Gestion des branches locales et distantes |
| **Commits** | Historique des commits |
| **Stash** | Liste des modifications mises de côté |

---

## Navigation de base

| Touche | Action |
|--------|--------|
| `↑/↓` | Navigation dans les listes |
| `←/→` | Changement de panneau |
| `h/j/k/l` | Navigation vim-style |
| `?` | Aide contextuelle |
| `q` | Retour/Quitter |

---

## Workflow basique

### 1. Gestion des fichiers

```bash
# Dans le panneau Files
space    # Ajouter/retirer un fichier du stage
a        # Tout ajouter au stage
d        # Voir les différences
```

### 2. Faire des commits

```bash
# Dans n'importe quel panneau
c    # Commit
C    # Commit avec message détaillé
```

### 3. Gestion des branches

```bash
# Dans le panneau Branches
n    # Nouvelle branche
b    # Checkout
M    # Merge
```

---

## Commandes essentielles

### Panneau Files
* `space` - Stage/unstage fichier
* `a` - Stage tout
* `d` - Voir les différences
* `D` - Reset fichier

### Panneau Branches
* `n` - Nouvelle branche
* `o` - Créer une pull request
* `M` - Merge
* `r` - Rebase

### Commandes globales
* `?` - Aide
* `q` - Retour
* `esc` - Retour
* `@` - Ouvrir le menu des commandes

> **Astuce** : Appuyez sur `?` dans n'importe quel panneau pour voir toutes les commandes disponibles.

---

## Prochaines étapes

* [Guide complet](usage.md) - Pour maîtriser toutes les fonctionnalités
* [Configuration](configuration.md) - Pour personnaliser LazyGit