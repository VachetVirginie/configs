
![alt text](https://newrelic.com/sites/default/files/2021-04/good-programmer-banner-final.jpg)

<p align="center">
  <a href="./.gitconfig">Git config</a> |
  <a href="./.zshrc">Zshrc config</a> |
  <a href="./iterm.md">Iterm</a> |
  <a href="./tricksMac.md">Terminal Tips & Tricks for Mac </a>
  <br><br>
  <!-- <img src="http://s.4cdn.org/image/title/105.gif"> -->
</p>

### Helpful commands

```source-shell
# Open finder in current folder.
open .

# Get wifi password.
brew install wifi-password
wifi-password

# Get project tree
brew install tree
tree

# Open web console 
Cmd + Option + K 

# Spectacle
brew install --cask spectacle

# Git 
Envie de faire un peu de ménage ? Voilà une commande pour faire le grand ménage dans vos branches en local. Remplacez « master » par le nom de la branche que vous voulez garder. Attention si les branches supprimées n’ont pas été push, elle seront perdues.

git branch | grep -v "master" | xargs git branch -D
```
