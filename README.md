# install-manjaro
Packages to build environment development in Linux Manjaro

## update Manjaro
`sudo pacman -Syu`

## install base-devel
`sudo pacman -S base-devel`

## install git
`sudo pacman -S git`

## install wget
`sudo pacman -S wget`

## install vim
`sudo pacman -S vim`

## install terminator
`sudo pacman -S terminator`

## install zsh
`sudo pacman -S zsh`

## install oh my zsh (https://blog.rocketseat.com.br/terminal-com-oh-my-zsh-spaceship-dracula-e-mais/)
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

## install spaceship
`git clone https://github.com/denysdovhan/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt"`

`ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"`

## install zinit
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/zdharma/zinit/master/doc/install.sh)"`

## install open java 11
`sudo pacman -S jdk11-openjdk`

## install maven
`sudo pacman -S maven`

## install yay
`sudo pacman -S yay`

## install vscode
`yay -S visual-studio-code-bin`

## install intellij
`sudo pacman -S intellij-idea-community-edition`

## install htop
`sudo pacman -S htop`

## install google chrome
`yay -S google-chrome`

## install aws sdk
`curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"`

`unzip awscliv2.zip`

`sudo ./aws/install`

`rm -rf awscliv2.zip && rm -rf aws`

## install dbeaver
`sudo pacman -S dbeaver`

## install docker
`sudo pacman -S docker`

## run docker without root (need reboot system `reboot`)
`sudo usermod -aG docker $USER`

## run image docker to mysql 5.6
`docker run --name mysql_5.6 -e MYSQL_DATABASE=mysql_5.6 -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql:5.6`

## install npm
`sudo pacman -S npm`

## install nodejs
`sudo pacman -S nodejs-lts-fermium`

## install yarn
`sudo npm install --global yarn`  

## install npx
`npm i npx`

## install discord
`sudo pacman -S discord`

## install insomnia
`yay -S insomnia`

`sudo ln -s /opt/insomnia/insomnia /usr/bin/insomnia`
