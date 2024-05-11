# nvim.profile
This is repostiroy with my neovim configuration. It was done based on tutorial from https://www.youtube.com/@ThePrimeTimeagen.

## Todo
- Descrbive components that are needed to deploy it
- Make ansible automation to prepare it automatically
- Add in automation easy adding lsp as arguments


## Issues
1. If you use WSL custom container on Windows, npm used in mason spin up new WSL shell session. Because of that you need to have setup /etc/wsl.conf file with
```
[user]
default=here_your_username
```
If you don't have you have situation that files in your home directory start to be installed from root account. 
