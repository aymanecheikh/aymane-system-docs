# DotFiles Management Project

## Tools

GNU Stow

## Research

Dotfiles are files that start with a dot:

--------------------
### Dotfile examples

e.g. .nvmrc, .zshrc, .bashrc, .gitignore, and .gitkeep
--------------------

True dotfiles are often used for configuration files, either project-wide or system-wide like zshrc.

But the term dotfiles has been expanded to mean all config files, such as ~/.config/nvim/*

People that are into 'ricing' their systems often have their dotfile repos publicly on GitHub. You can learn from their Vim configurations, copy their transparent windows or tiling animations without having to ask for any details.

In order to start my own dotfile repo, I would have the following options, in order of least efficient to most efficient:

### Option 1 - Copy/Paste Config files

This is not only very labour intensive and unsustainable, but also extremely risky.

### Option 2 - Create Symbolic Links

This can be done with:
```ln -s ~/.dotfiles/nvim ~/.config/nvim```

Symbolic links, or symlinks, are the way that Linux implements shortcuts like you have in Windows. You can have a symlink on your desktop that points to a configuration file. And then each change you make at ~/dotfiles/* will be reflected in ~/.config/*

While symbolic links are certainly the right approach, and creating symlinks for each folder or file within a dedicated repository for centralized configuration management would be a great learning curve, it is still manual in the sense that I would have to keep track of each configuration, which would grow into large maintenance task, particularly as my operating system evolves.

### Option 3 - Stow - Symlink Automation

With stow, we don't have to create our symlinks by ourselves.

We start off by creating a folder called dotfiles in our Home directory, initialize git, and begin stowing.

## Project

### Config Checklist

Hyprland          | ~/.config/hypr/

waybar            | ~/.config/waybar/

rofi              | ~/.config/rofi/

dunst             | ~/.config/dunst/

swaylock-effects  | configured in hypr 

swww              | systemwide?

