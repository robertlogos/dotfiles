FEDORA ATOMIC
-------------

*Paquetes adicionales

rpm-ostree install alacritty chezmoi hyprlauncher hyprshutdown powertop tmux uv wlogout zoxide zsh

*Cambiar shell (tmux lo necesita)
chsh -s /bin/zsh

*Flatpaks
 - flatpak install flathub com.visualstudio.code (meter link en .local/bin)

*Otros
 - Configuraciones del grub2 (en atomic hay que crear un user.cfg)
 - Instalar pCloud (APPImage en .local/bin)
 - Copiar .ssh
 - Crear distrobox e instalar azure-cli dentro del mismo exportandolo al inmutable: distrobox-export --bin /usr/bin/az --export-path ~/.local/bin
 
