---
id: ArchLinux
aliases: []
tags: []
---

# Minimal Package List for Backup / Reinstallation

## Package Install Command

pacman -S base base-devel linux linux-firmware linux-headers sudo networkmanager hyprland waybar rofi dunst swaylock-effects swww xdg-desktop-portal-hyprland git lazygit neovim tmux kitty zsh starship brightnessctl usbutils htop jq wget xdg-utils xdg-desktop-portal-gtk pipewire-alsa pipewire-pulse sof-firmware alsa-utils papirus-icon-theme qt5ct qt6ct nwg-look firefox yay-bin


## Core System Packages

base                        | Essential Arch System
base-devel                  | Required for compiling AUR packages
linux                       | Kernel
linux-firmware              | Drivers
linux-headers               | Drivers
sudo                        | Root permissions
networkmanager              | Internet connection

## System Utilities

brightnessctl               | Adjust screen brightness
usbutils                    | USB debugging
htop                        | System monitor
jq                          | JSON processing
wget                        | Download files
xdg-utils                   | Open files/apps
xdg-desktop-portal-gtk      | Ensures Wayland compatibility

pipewire-alsa               | Audio | Device & Server Interaction
pipewire-pulse              | Audio | Server
sof-firmware                | Audio | Intel Sound Chip compatibility
alsa-utils                  | Audio | Hardware

## Package Manager

yay-bin                     | AUR helper

## Hyprland Core

hyprland                    | Wayland window manager
waybar                      | Status bar
rofi                        | App launcher
dunst                       | Notifications
swaylock-effects            | Lock screen
swww                        | Wallpaper daemon
xdg-desktop-portal-hyprland | Ensures Wayland compatibility

## Theming

papirus-icon-theme          | Icons
qt5ct qt6ct                 | Configure Qt apps
nwg-look                    | GTK theming for Wayland

## Browser

firefox                     | Main Browser


## Development Tools

git                         | Version control
lazygit                     | GUI for git
neovim                      | Code editor
tmux                        | Terminal multiplexing
kitty                       | Fast terminal
zsh                         | Shell
starship                    | Shell prompt
