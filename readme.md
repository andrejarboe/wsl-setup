# Setup

##

https://learn.microsoft.com/en-us/windows/wsl/install:

wsl --install

## udate

sudo apt-get update

sudo apt-get upgrade


## make code folder

cd ~

mkdir ubuntuCode

## Bash 

* back up .bashrc 
* cd ~
* cp .bashrc .bashrc.backup
* https://github.com/andresgongora/synth-shell
* sudo apt install fonts-powerline
* inatall hack font
    * https://github.com/source-foundry/Hack-windows-installer/releases/tag/v1.6.0
    * reboot
* Fancy bash prompt:
    *  git clone --recursive https://github.com/andresgongora/synth-shell.git
    * chmod +x synth-shell/setup.sh
    * cd synth-shell
    * ./setup.sh
        * [i] install 
        * [u] current user only
        * Install synth-shell-greeter? (Y/n): n
        * Install synth-shell-prompt? (Y/n): y
        * [??]  Install better-ls? (Y/n): n
        * [??]  Install alias? (Y/n): n
        * [??]  Install better-history? (Y/n): n

## install nvm
https://github.com/nvm-sh/nvm

## Configure git:

git config --global user.name "Andre Jarboe"

git config --global user.email "andrejarboe@gmail.com"

git config --global init.defaultBranch main

git config --global color.ui auto

## Verify
git config --get user.name

git config --get user.email

## Create an SSH Key
ls ~/.ssh/id_rsa.pub

ssh-keygen -t rsa -C "andrejarboe@gmail.com" -f ~/.ssh/id_rsa -P ""

## Create an SSH Key
ls ~/.ssh/id_rsa.pub

ssh-keygen -t rsa -C "andrejarboe@gmail.com" -f ~/.ssh/id_rsa -P ""

## Link Your SSH Key with GitHub
cat ~/.ssh/id_rsa.pub

Highlight and copy the output, which starts with ssh-rsa and ends with your email address.

Now, go back to GitHub in your browser window and paste the key you copied into the key field. Then, click Add SSH key. You’re done! You’ve successfully added your SSH key!

## Test it