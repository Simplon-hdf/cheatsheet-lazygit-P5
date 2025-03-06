# Configuration initiale de Lazygitlg

Lazygit stocke ses fichiers de configuration dans :
- 📂 **Linux/macOS** : `~/.config/lazygit/config.yml`
- 📂 **Windows** : `C:\Users\VotreNom\AppData\Roaming\lazygit\config.yml`

---
##  Créer et modifier le fichier de configuration
Avant de personnaliser Lazygit, il faut créer son fichier de configuration :

```sh
mkdir -p ~/.config/lazygit
nano ~/.config/lazygit/config.yml
```

Ce fichier vous permet de modifier l'apparence et le comportement de Lazygit.

---
##  Exemple de configuration avancée

Voici une configuration avancée avec personnalisation de l'interface et des raccourcis :

```yaml
gui: 
  theme:
    activeBorderColor:
      - cyan
      - bold
    inactiveBorderColor:
      - white
  showIcons: true
  showFileTree: true
  nerdFontsVersion: "3"
  
git:
  paging:
    colorArg: always
    pager: delta --dark --paging=never
  branchLogCmd: "git log --oneline --graph --decorate --color=always"

keybinding:
  universal:
    quit: "q"
    return: "<esc>"
  files:
    commitChanges: "c"
```

### ** Explication des paramètres :**
- **GUI :**
  - Affichage des **icônes** et de l'**arborescence des fichiers**.
  - Personnalisation des **bordures** avec des couleurs distinctes.
  - Utilisation des **Nerd Fonts** pour une meilleure compatibilité.
- **Git :**
  - Activation de `delta` pour une meilleure mise en page des logs.
  - Affichage des commits avec `git log --oneline --graph --decorate`.
- **Keybinding :**
  - `q` pour quitter.
  - `<esc>` pour revenir en arrière.
  - `c` pour valider les modifications.

---
##  Ajout d’un alias pour un accès rapide

Créer un alias `lg` pour exécuter `lazygit` plus rapidement :

**Sur Bash :**
```sh
echo 'alias lg="lazygit"' >> ~/.bashrc
source ~/.bashrc
```

**Sur Zsh :**
```sh
echo 'alias lg="lazygit"' >> ~/.zshrc
source ~/.zshrc
```

**Sur Windows (PowerShell) :**
```powershell
New-Alias -Name lg -Value lazygit
```

Si l'alias ne fonctionne pas immédiatement, redémarrez votre terminal.

---
###  **Résumé des améliorations**
- Correction des erreurs de formatage YAML.
- Explications détaillées pour chaque paramètre.
- Ajout des alias pour PowerShell sur Windows.
- Amélioration de la lisibilité avec une meilleure structuration.

Avec ces ajustements, votre Lazygit sera plus efficace et mieux personnalisé !

