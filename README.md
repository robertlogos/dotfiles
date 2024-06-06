# .dotfiles

## Setup environment

Install `homebrew` (macOS), `zsh`, `tmux`, `git`, `chezmoi`,  and basic tools:

### Commandline tools
- zoxide
- fzf
- vim
- neovim
- bat
- tree
- lsd
- rg
- mc
- thefuck

### Development tools
- asdf
- podman
- maven
- vscode

### Fonts
- font-jetbrains-mono-nerd-font
- font-victor-mono-nerd-font
- font-meslo-lg-nerd-font
- font-iosevka-nerd-font
- font-inconsolata-nerd-font
- font-ubuntu-mono-nerd-font

## Install .dotfiles

Download .dotfiles

    chezmoi init https://github.com/robertlogos/dotfiles.git
    chezmoi apply

Edit following configurations to your desired specifics:

- `~/.zshenv` environment variables
- `~/.vimrc` background colors (dark|light)
- `~/.config/nvim/init.lua` neovim
- `~/.config/tmux/tmux.conf` tmux
- `~/.config/alacritty/alacritty.toml` alacrittiy

Configure p10k prompt line

    p10k configure

## Working with .dotfiles and chezmoi

After editing the dotfiles

    chezmoi add <FILE>

Check for differences

    chezmoi diff
    chezmoi diff <FILE>

Undo changes / Apply from repository

    chezmoi apply
    chezmoi apply <FILE>


Set remote url

    chezmoi cd
    git remote set-url origin https://robertlogos:<API_KEY>@github.com/robertlogos/dotfiles.git


Push updates into repository

    chezmoi cd
    git add .
    git commit -m "<COMMIT_MESSAGE>"
    git push -u origin main

Update repository
    
    chezmoi git pull


















