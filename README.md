# shua-bspwm
A custom bspwm theme

First, clone the git repository
```
git clone https://github.com/Shua24/shua-bspwm.git
```
# Setting up bspwm:

Before copying the config files, install the dependencies first.
#### Arch-based distros:
If you use paru:
```
paru -S bspwm rofi polybar lxsession picom nitrogen pywal ttf-roboto qt5-styleplugins lxappearance gnome-materia-theme xterm
```
If you're using yay:
```
yay -S bspwm rofi polybar lxsession picom nitrogen pywal ttf-roboto qt5-styleplugins lxappearance gnome-materia-theme
```
(You can also edit the bspwm keybinds in `~/.config/sxhkd/sxhkdrc` before switching to bspwm to add a keybind for `rofi` and other programs)

#### Copying the icons
1) Extract all icons.
2) Copy `Win7Build=dark-cursors` and `Cyan-Breeze-Dark-Icons` into the `~/.icons` directory.

The cheater method (Assuming you cloned all the config files in the home directory):
```
cp ~/bspwm-shua/Cyan-Breeze-Dark-Icons/ ~/.icons/Cyan-Breeze-Dark-Icons/
cp ~/bspwm-shua/Win7Bulid-dark-cursors/ ~/.icons/Win7Bulid-dark-cursors/
```
Before you copy the config files, setup the dark theme and icons by opening `lxappearance`. Don't forget to setup a wallpaper using `nirogen` by adding a directory to the preferences.

Add this to `/etc/environment`
```
XDG_CURRENT_DESKTOP=Unity
QT_QPA_PLATFORMTHEME=gtk2
```

#### Copying all the config files

1) Copy `bspwmrc` to `~/.config/bspwm/bspwmrc`
2) Copy `bashrc` to `~/.bashrc`
3) copy `polybar-config` to `~/.config/polybar/config

The cheater method (Assuming you cloned all the config files in the home directory):
```
cp ~/bspwm-shua/bashrc ~/.bashrc
cp ~/bspwm-shua/bspwmrc ~/.config/bspwm/bspwmrc
cp ~/bspwm-shua/polybar-config ~/.config/polybar/config
```

(Note: the `source .bashrc` command is not yet executed unless you're done setting up bspwm).

# Finishing commands

1) Match the terminal and text CLI text editor color scheme with wallpaper using wal:
```
wal -i path/to/your/wallpaper.png
```
Usually the folder for your wallpapers is in `/usr/share/backgrounds/` directory.

2) Sourcing `.bashrc`
```
source .bashrc
```
3) Restart bspwm by pressing `mod + R`
4) Done.

Icons:
1) Cyan-Breeze-Dark-Icons https://www.gnome-look.org/s/Gnome/p/1483458
2) Win7Build-dark-cursors https://www.gnome-look.org/p/1437431/
