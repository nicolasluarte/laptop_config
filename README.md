# laptop_config
my personal laptop configuration

## PDF
```
yay -S zathura-pdf-mupdf
```

## Pandoc
```
yay -S pandoc
```

## Python
```
sudo pacman -S python
sudo pacman -S python-pip
sudo pacman -S ipython
```

## R
```
sudo pacman -S r
sudo pacman -S gcc-fortran
```
Add this to Rprofile
```
touch .Rprofile
## Set CRAN mirror:
local({
  r <- getOption("repos")
  r["CRAN"] <- "https://cloud.r-project.org/"
  options(repos = r)
})
```

## NeoVim
```
sudo pacman -S neovim
git clone https://github.com/nicolasluarte/nvim-config
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
pip3 install --user neovim-remote
pip3 install --user pynvim

```

## alacritty
Just do a symlink of this into ~/.config/alacritty/
```
sudo pacman -S alacritty
git clone https://github.com/nicolasluarte/alacritty_config
```

## ZSH
```
sudo pacman -S zsh
yay -S zsh-autosuggestions
```
Install oh-my-zsh
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
Clone repo to .oh-my-zsh/custom/plugins
```
git clone https://github.com/zsh-users/zsh-autosuggestions
```
Add the plugin to the list of plugins inside .zshrc
```
plugins=(zsh-autosuggestions)
```

## Screenshot
```
yay -S flameshot
```

## FFMPEG
```
sudo pacman -S ffmpeg
```

## Music player
```
sudo pacman -S cmus
```
