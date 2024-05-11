# nvim.profile
This is repostiroy with my neovim configuration. It was done based on tutorial from https://www.youtube.com/@ThePrimeTimeagen.

## Todo
- Descrbive components that are needed to deploy it
- Make ansible automation to prepare it automatically
- Add in automation easy adding lsp as arguments

## Manual Installation
1. Install packer
```
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
```
2. Git clone this repo
```
git clone https://github.com/DawidAdamski/nvim.profile\
 ~/.config/nvim/
```
3. Load packer lua.
Execute nvim, using :Ex go to packer.lua and load it with :so. After :PackerSync to download dependepncies.
4. To make working grep feature install ripgrep

It was tested in RHEL 8 and Fedora 38

## Issues
1. If you use WSL custom container on Windows, npm used in mason spin up new WSL shell session. Because of that you need to have setup /etc/wsl.conf file with
```
[user]
default=here_your_username
```
If you don't have you have situation that files in your home directory start to be installed from root account. 
