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

## add yaourt
`sudo pacman -S --needed base-devel git wget yajl`

## clone and install package-query that allows to build and run yaourt
`git clone https://aur.archlinux.org/package-query.git && cd package-query/`

## compile and install package-query
`makepkg -si`

## return folder
`cd ..`

## clone and install yaourt
`git clone https://aur.archlinux.org/yaourt.git && cd yaourt/`

## compile and install yaourt
`makepkg -si`

## return folder
`cd ..`

## remove folders
`sudo rm -dR yaourt/ package-query/`

## install open java 11
`sudo pacman -S jre11-openjdk-headless jre11-openjdk jdk11-openjdk openjdk11-doc openjdk11-src`

## install maven
`sudo pacman -S maven`

## install vscode
`yaourt visual-studio-code-bin`

## install google chrome
`yaourt -S google-chrome`

## install aws sdk
`curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"`

`unzip awscliv2.zip`

`sudo ./aws/install`

`rm -rf awscliv2.zip && rm -rf aws`

## install dbeaver
`pamac install dbeaver && sudo pacman -S dbeaver`

## install docker
`sudo pacman -S docker`

## run docker without root (need reboot system `reboot`)
`sudo usermod -aG docker $USER`

## run image docker to mysql 5.6
`docker run --name mysql_5.6 -e MYSQL_DATABASE=mysql_5.6 -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql:5.6`
