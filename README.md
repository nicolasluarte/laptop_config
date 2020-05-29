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
```

## R
```
sudo pacman -S r
sudo pacman -S gcc-fortran
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
