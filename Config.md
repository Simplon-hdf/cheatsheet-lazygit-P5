#Configuration initiale de Lazygitlg#

Lazygit stocke ses fichiers de configuration dans :

 📂 Linux/macOS : ~/.config/lazygit/config.yml
 
 📂 Windows : C:\Users\VotreNom\AppData\Roaming\lazygit\config.yml

 ## Créer et modifier le fichier de configuration ##
mkdir -p ~/.config/lazygit
nano ~/.config/lazygit/config.yml


### Exemple de configuration avancée : ###

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

Points clés de cette configuration :
 -Activation des icônes et des polices Nerd Fonts
 -Personnalisation des couleurs de l’interface
 -Utilisation de delta pour un affichage amélioré des logs Git
 -Raccourcis personnalisés pour les actions courantes

##Ajout d’un alias pour un accès rapide##

Pour exécuter Lazygit avec lg, ajoutez cet alias :
echo 'alias lg="lazygit"' >> ~/.bashrc
source ~/.bashrc

Pour Zsh (Oh My Zsh) :
echo 'alias lg="lazygit"' >> ~/.zshrc
source ~/.zshrc

