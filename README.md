# dotfiles
configs of my tools and etc.
## Install
### Install GitHub CLI
```zsh
brew install gh
```
```bash
sudo apt install gh
```
```PowerShell
winget install --id Github.cli
```
#### Login in GitHub CLI
```zsh
gh auth login
```
### Clone repo
```zsh
gh repo clone xm4dn355x/dotfiles
```
### Install dotfiles
```zsh
./install
```
Have fun!
# dotfiles structure
```yml
dotfiles:
    - steps:
        - base.yml: "basic universal configs"
        - macos.yml: "MacOS specific configs"
        - pyton.yml: "Install python environment"
        - neovim.yml: "NeoVim configs"
        - zsh.yml: "ZSH shell configs"
    - config:
        - starship.toml
        - zsh:
            - .zshrc
            - .zshenv
            - aliases.zsh
        - tmux:
            - .tmux.conf
    - Brewfile: "brew bundle file"
    - install: "Main script for dotfiles installation"
    - install.conf.yml: "Main script configs"
```
