# shua-bspwm
A list of config files in my bspwm settings

# Setting up bspwm:

Before copying the config files, install the dependencies first.
#### Arch-based distros (using paru):
```
paru -S bspwm rofi polybar lxsession picom nitrogen pywal ttf-roboto qt5-styleplugins lxappearance gnome-materia-theme xterm
```
If you're using yay:
```
yay -S bspwm rofi polybar lxsession picom nitrogen pywal ttf-roboto qt5-styleplugins lxappearance gnome-materia-theme
```
(You can also edit the bspwm keybinds in `~/.config/sxhkd/sxhkdrc`)

Add this to `/etc/environment`
```
XDG_CURRENT_DESKTOP=Unity
QT_QPA_PLATFORMTHEME=gtk2
```

#### Copying all the files

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

1) Match the terminal and text CLI text editor color scheme with  wallpaper using wal:
```
wal -i path/to/your/wallpaper.png
```

2) Sourcing `.bashrc`
```
source .bashrc
```
3) Restart bspwm by pressing `mod + R`
4) Done.
