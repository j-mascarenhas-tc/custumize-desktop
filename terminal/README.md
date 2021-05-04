# Terminal Setup with Zsh and Tmux on Linux

## Install Bash-completion

`apt-get install bash-completion`

## Install ZSH

Ubuntu

`sudo apt update && sudo apt install zsh`

Change default shell to zsh

`chsh -s /bin/zsh`

Log out and log in again to apply

Open you terminal and press (2)

## install OH my Zsh

`sudo apt install git`

`curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh; zsh`

## install Zsh-Autosuggestions

`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

## install Zsh-Syntax-Highlighting

`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

Add to zsh config

`vim /root/.zshrc`

plugins=(
git
zsh-syntax-highlighting
zsh-autosuggestions
)

## install Powerlevel10k

install fonts

`sudo apt install -y fonts-font-awesome`

clone repository

`git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`

Set ZSH_THEME="powerlevel10k/powerlevel10k" in ~/.zshrc.

Close and open terminal and answer the questions

## install Tmux

`sudo apt install tmux`

Copy tmux/.tmux.conf to ~/.tmux.conf
