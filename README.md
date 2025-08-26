From scratch

```shell
git init --bare "$HOME/.dotfiles"
alias dot='/usr/bin/git --git-dir="$HOME/.dotfiles" --work-tree="$HOME"'
dot config --local status.showUntrackedFiles no
```

Clone

```shell
git clone --bare https://github.com/eddy-geek/dotfiles-bare "$HOME/code/GEEK/dotfiles-bare.git"
alias dot='/usr/bin/git --git-dir="$HOME/code/GEEK/dotfiles-bare.git" --work-tree="$HOME"'
dot checkout # this might warn about overwritting files
dot config --local status.showUntrackedFiles no
```

Dependencies:

```
# ohmyz.sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# tools
