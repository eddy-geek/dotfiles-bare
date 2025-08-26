From scratch

```shell
git init --bare "$HOME/.dotfiles"
alias dot='/usr/bin/git --git-dir="$HOME/.dotfiles" --work-tree="$HOME"'
dot config --local status.showUntrackedFiles no
```

Clone

```shell
git clone --bare https://github.com/eddy-geek/dotfiles-bare "$HOME/code/GEEK/dotfiles"
alias dot='/usr/bin/git --git-dir="$HOME/code/GEEK/dotfiles" --work-tree="$HOME"'
dot checkout # this might warn about overwritting files
dot config --local status.showUntrackedFiles no
```
