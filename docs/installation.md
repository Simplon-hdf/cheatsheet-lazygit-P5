# Installation de LazyGit

> **Prérequis** : Git doit être installé sur votre système avant de procéder à l'installation de LazyGit.

---

## Windows

### Installation via Chocolatey

```powershell
# Installation en une ligne
choco install lazygit
```

1. [Installez Chocolatey](https://chocolatey.org/install) si nécessaire
2. Ouvrez PowerShell en administrateur
3. Exécutez la commande d'installation
4. Vérifiez avec `lazygit --version`

> 📺 [Voir le tutoriel vidéo](https://www.youtube.com/watch?v=M-A7os3qEiM&t=2s)

### Installation via Scoop

```powershell
# Ajout du bucket et installation
scoop bucket add extras
scoop install lazygit
```


1. [Installez Scoop](https://scoop.sh/) si nécessaire
2. Ouvrez PowerShell
3. Ajoutez le bucket extras
4. Installez LazyGit
5. Vérifiez avec `lazygit --version`

> 📺 [Voir le tutoriel vidéo](https://www.youtube.com/watch?v=sZS7mG_zhaw)

---

## Linux

### Ubuntu/Debian

```bash
# Installation automatique
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": *"v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/v${LAZYGIT_VERSION}/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit -D -t /usr/local/bin/

# Vérification
lazygit --version
```

### Arch Linux

| Version | Commande | Description |
|---------|----------|-------------|
| **Stable** | `sudo pacman -S lazygit` | Version recommandée |
| **Dev** | Via [AUR](https://aur.archlinux.org/packages/lazygit-git/) | Dernières fonctionnalités |

> **Note** : La version stable est recommandée pour la plupart des utilisateurs.

---

## macOS

### Installation via Homebrew

| Source | Commande | Note |
|--------|----------|------|
| **Dépôt officiel** | `brew install jesseduffield/lazygit/lazygit` | Recommandé |
| **Dépôt principal** | `brew install lazygit` | Alternative |

> **Info** : Le dépôt officiel fournit des mises à jour plus fréquentes.

---

## Vérification de l'installation

```bash
# Vérifiez que LazyGit est correctement installé
lazygit --version
```

> **Succès** : Si la commande affiche la version, LazyGit est prêt à être utilisé !
