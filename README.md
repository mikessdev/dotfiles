# My Dot files:



## Automate this

```sh
### update 
sudo apt update && sudo apt upgrade -y
sudo apt install build-essential


### Instalando coisas básicas
sudo apt-get install wget curl neofetch zsh fonts-firacode unzip snapd flameshot gnome-tweaks

### Fonts 

#### JetBrainsMono
wget -O JetBrainsMono.zip https://github.com/JetBrains/JetBrainsMono/archive/refs/tags/v2.304.zip
unzip JetBrainsMono.zip -d ~/.local/share/fonts
sudo rm JetBrainsMono.zip





### Oh My ZSH Setup
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"

#### plugins
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/MichaelAquilina/zsh-you-should-use.git $ZSH_CUSTOM/plugins/you-should-use
git clone https://github.com/fdellwing/zsh-bat.git $ZSH_CUSTOM/plugins/zsh-bat

### starship 
curl -sS https://starship.rs/install.sh | sh





### Setup dotfiles
git clone --recurse-submodules https://github.com/mikessdev/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig




### auto-cpufreq
git clone https://github.com/AdnanHodzic/auto-cpufreq.git
cd auto-cpufreq && sudo ./auto-cpufreq-installer

### google chrome 
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
sudo rm google-chrome-stable_current_amd64.deb

### vscode 
sudo apt install software-properties-common apt-transport-https wget
wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"
sudo apt install code

### obsidian 
sudo snap install obsidian
cd ~/dev && git clone git@github.com:mikessdev/ObsidianNotes.git

### dbeaver-ce 
wget -O dbeaver-ce.deb https://dbeaver.io/files/dbeaver-ce_latest_amd64.deb
sudo dpkg -i dbeaver-ce.deb
sudo rm dbeaver-ce.deb

### obs studio 
sudo apt install v4l2loopback-dkms
sudo add-apt-repository ppa:obsproject/obs-studio
sudo apt update
sudo apt install obs-studio


### Docker e Docker compose 
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-pt

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04-pt


### zoom 
wget https://zoom.us/client/latest/zoom_amd64.deb
sudo dpkg -i zoom_amd64.deb
sudo rm zoom_amd64.deb

### nvm 
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash


### vscode config
cat ./vscode/extensions.txt | xargs -n 1 code --install-extension



### Finalização
mkdir ~/dev && mkdir ~/playground 

´´´




## todo

### Node
[X] - Install nvm 

### Nerd Font 

[X] - install Firacode 
[X] - install JetBrainsMono

### Oh My ZSH

[X] - Install plugin git 
[X] - install zsh-autosuggestions
[X] - install zsh-syntax-highlighting
[X] - Install starship 


### Programas 
[ ] - spotify 
[X] - vscode 
[X] - auto-cpufreq
[X] - dbeaver 
[X] - google chrome 
[X] - Obsidian 
[X] - Flameshot 
[X] - ObsStudio
[X] - Docker && Docker compose 
[ ] - Tandem 
[ ] - Zoom 







