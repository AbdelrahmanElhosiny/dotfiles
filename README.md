# dotfiles

to add "stow --adopt -vt ~ app-name"
to load "stow app-name"

add gnome-extensions
dconf dump /org/gnome/shell/extensions/ > extension-settings.dconf

load gnome-extensions
dconf load /org/gnome/shell/extensions/ < extension-settings.dconf

add dconf
dconf dump / > all-dconf.dconf

load dconf
dconf load / < all-dconf.dconf
