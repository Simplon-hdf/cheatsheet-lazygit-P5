## Comment ça marche 

L'écran est divisé en plusieurs zones :
- **Files** : Vos fichiers modifiés et en attente de commit
- **Branches** : Toutes vos branches (locales et distantes)
- **Commits** : L'historique de vos commits
- **Stash** : Vos modifications mises de côté
- **Status** : L'état de votre dépôt

## Se déplacer dans l'interface 

### Les bases 
- `tab` → Change de zone
- `h/j/k/l` ou flèches → Se déplace dans la zone active
- `?` → Affiche l'aide
- `q` → Quitte l'application
- `esc` → Retourne en arrière

### Ajuster l'affichage 
- `+` / `-` → Agrandit ou réduit la zone
- `_` → Passe en plein écran

## Les commandes de base 

### Gérer vos fichiers 

```bash
espace    # Ajoute/Retire un fichier du prochain commit
a         # Ajoute/Retire tous les fichiers du prochain commit
d         # Annule les changements du fichier
e         # Ouvre le fichier dans votre éditeur
o         # Ouvre le fichier avec le programme par défaut
```

### Gérer vos commits 

```bash
c         # Crée un commit
A         # Modifie le dernier commit
z         # Annule la dernière action
ctrl+z    # Rétablit la dernière action annulée
```

### Gérer vos branches 

```bash
n         # Crée une branche
o         # Change de branche
O         # Cherche et change de branche
M         # Fusionne des branches
P         # Récupère les changements du serveur
p         # Envoie vos changements au serveur
```

## Fonctions avancées 

### Rebase interactif 

Choisissez un commit et tapez `i` pour démarrer le rebase :

```bash
s         # Fusionne avec le commit du dessus en gardant les messages
f         # Fusionne avec le commit du dessus sans garder le message
d         # Supprime le commit
e         # Arrête pour modifier le commit
ctrl+j/k  # Déplace le commit vers le haut/bas
```

### Cherry-pick 

```bash
shift+c   # Copie un commit
shift+v   # Colle le commit copié
```

### Stash

```bash
s         # Met de côté vos changements
g         # Récupère les changements mis de côté
d         # Supprime les changements mis de côté
shift+S   # Autres options pour la mise de côté
```


## Comprendre les couleurs de l'interface

### Les commits
- 🟢 **Vert** : Le commit est dans votre branche principale
- 🟡 **Jaune** : Le commit n'est pas dans votre branche principale
- 🔴 **Rouge** : Le commit n'est pas encore envoyé au serveur

### Raccourcis importants 
- `m` → Lance un rebase interactif
- `shift+P` → Pousse (push) les changements vers le dépôt distant
- `shift+?` → Affiche tous les raccourcis disponibles

## Conseils 

- Appuyez sur `?` dans chaque zone pour voir les commandes disponibles
- Utilisez les raccourcis clavier, c'est plus rapide
- Le rebase interactif est plus facile avec LazyGit qu'en ligne de commande
