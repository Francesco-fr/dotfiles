# Francesco's dotfiles

Stuff from my arch linux instance, feel free to use my stuff.
You will probably need to edit some of the config files to get them working for you.

## Screenshots

![Screenshot1](https://pix.milkywan.fr/IsQW0UiA.png)

![Screenshot2](https://pix.milkywan.fr/ZBmnTr3h.png)

## Move configs

```bash
cp -r config/* ~/.config/
```

## Packages to install

### Packages

```bash
yay -S hyprland sddm-git xdg-desktop-portal-hyprland eww-wayland hyprpaper hyprshot kitty nemo p7zip-gui polkit-kde-agent pyprland waybar wofi btop neofetch pipes.sh qt5-wayland qt6-wayland
```

### Fonts
```bash
yay -S ttf-jetbrains-mono ttf-nerd-fonts-symbols 
```

### Audio

```bash
yay -S pipewire pipewire-alsa pipewire-audio pipewire-jack pipewire-pulse wireplumber noise-suppression-for-voice pavucontrol
```

## GTK

```bash
git clone https://github.com/dracula/gtk.git
cp -r gtk ~/.themes/Dracula
gsettings set org.gnome.desktop.interface gtk-theme 'Dracula'
rm -r gtk
wget https://github.com/dracula/gtk/files/5214870/Dracula.zip
unzip Dracula.zip
rm Dracula.zip
cp -r Dracula ~/.icons/Dracula/
gsettings set org.gnome.desktop.interface icon-theme 'Dracula'
rm -r Dracula
```
