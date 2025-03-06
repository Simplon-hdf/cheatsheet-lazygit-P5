## Installation 

### Windows 

#### Via [Chocolatey](https://chocolatey.org/install)

Videos d'installation de [ChocoLatey](https://www.youtube.com/watch?v=M-A7os3qEiM&t=2s)

```bash
# Installation de lazygit
choco install lazygit
```

#### via scoop [Scoop](https://scoop.sh/)

vidéos d'installation [scoop](https://www.youtube.com/watch?v=sZS7mG_zhaw)

```bash
# Ajouter le bucket extras
scoop bucket add extras

# Installer lazygit
scoop install lazygit 
```

### Linux 

#### via Ubuntu

```bash 
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | \grep -Po '"tag_name": *"v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/download/v${LAZYGIT_VERSION}/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit -D -t /usr/local/bin/
```

Vérifier que la bonne version de lazygit a été installée:

```bash
lazygit --version
```


#### via Arch Linux 

Les paquets pour Arch Linux sont accessibles via pacman et l'AUR (Arch User Repository).

Deux versions sont disponibles : la version stable, qui est basée sur la dernière version officielle, et la version git, qui se construit à partir des derniers commits.

Stable :  ``` sudo pacman -S lazygit```

[Version Developpement](https://aur.archlinux.org/packages/lazygit-git/)

### macOS 

#### via Homebrew 

Normalement, la formule de LazyGit est disponible dans le dépôt principal de Homebrew, mais nous vous conseillons d'ajouter notre dépôt pour obtenir une version mise à jour plus fréquemment. Elle fonctionne aussi sous Linux.

Avec notre dépôt :
```bash 
brew install jesseduffield/lazygit/lazygit
```

via le dépôt principal :
```bash
brew install lazygit
```
