# capuk-nix-home-manager


## guides
- https://ghedam.at/24353/tutorial-getting-started-with-home-manager-for-nix
- https://regolith-desktop.com/docs/using-regolith/install/

## todo
- bash aliases 
- i3 configs

## manual
- login firefox
- login password manager
- add ssh key 
- set kagi default, update layout firefox
- install rambox https://rambox.app/download-windows/
- install beeper https://www.beeper.com/download

## shell
```
# basic
sudo apt install vim curl

# setup i3
### follow https://regolith-desktop.com/docs/using-regolith/install/
sudo apt install i3xrocks-focused-window-name i3xrocks-rofication i3xrocks-info i3xrocks-app-launcher i3xrocks-memoryregolith-look-dracula
regolith-look set dracula
sudo rm -rf /usr/share/regolith/*

# setup nix
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

## reference
- https://www.reddit.com/r/NixOS/comments/z11yji/example_starter_configs/ | Example Starter Configs : r/NixOS
- https://github.com/Panadestein/nixos-config | GitHub - Panadestein/nixos-config: A minimalist NixOS config
- https://github.com/baitinq/nixos-config | GitHub - Baitinq/nixos-config: My Personal Nix/NixOS Configuration.
- https://github.com/dmadisetti/.dots | GitHub - dmadisetti/.dots: just my .dotfiles
- https://github.com/Misterio77/nix-starter-configs | GitHub - Misterio77/nix-starter-configs: Simple and documented config templates to help you get started with NixOS + home-manager + flakes. All the boilerplate you need!
- https://github.com/Th0rgal/horus-nix-home/blob/master/packages/main.nix | horus-nix-home/packages/main.nix at master · Th0rgal/horus-nix-home
