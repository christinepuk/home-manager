## guides
https://ghedam.at/24353/tutorial-getting-started-with-home-manager-for-nix
https://regolith-desktop.com/docs/using-regolith/install/

## manual
- login firefox
- login password manager
- add ssh key 

## installed 
```
sudo apt install vim curl
sudo apt install i3xrocks-focused-window-name i3xrocks-rofication i3xrocks-info i3xrocks-app-launcher i3xrocks-memoryregolith-look-dracula
regolith-look set dracula
export EDITOR=vim
curl -L https://nixos.org/nix/install | sh
nix
nix-channel --add https://github.com/nix-community/home-manager/archive/master.tar.gz home-manager
nix-channel --update
nix-shell '<home-manager>' -A install
home-manager
cd $HOME/.config/
git clone git@github.com:christinepuk/home-manager.git
home-manager switch
```
