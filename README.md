# shua-bspwm
A custom bspwm theme for beginners.

First, clone the git repository.
```
git clone --branch full https://github.com/Shua24/shua-bspwm.git
```
# Setting up bspwm

Before copying the config files, install the dependencies first.
#### Arch-based distros:
If you use paru:
```
paru -S bspwm rofi polybar lxsession picom nitrogen gnome-screenshot pywal ttf-roboto qt5-styleplugins lxappearance materia-gtk-theme betterlockscreen sakura -y
```
If you're using yay:
```
yay -S bspwm rofi polybar lxsession picom nitrogen gnome-screenshot pywal ttf-roboto qt5-styleplugins lxappearance materia-gtk-theme betterlockscreen sakura -y
```
(You can also edit the bspwm keybinds in `~/.config/sxhkd/sxhkdrc` before switching to bspwm to add a keybind for `rofi` and other programs).


Before you copy all the icons and config files, set the terminal font to Roboto Mono.

#### Copying the icons
1) Extract all icons.
2) Copy `Win7Build-dark-cursors` and `Neonyt-Dark-Icons` into the `~/.icons` directory.

The cheater method (Assuming you cloned all the config files in the home directory):
```
cp ~/shua-bspwm/Neonyt-Dark-Icons/ ~/.icons/Cyan-Breeze-Dark-Icons/
cp ~/shua-bspwm/Win7Bulid-dark-cursors/ ~/.icons/Win7Bulid-dark-cursors/
```
Before you copy the config files, setup the dark theme and icons by opening `lxappearance`. Don't forget to setup a wallpaper using `nitrogen` by adding a directory to the preferences. After that, set a default lockscreen for your bspwm setup.
```
betterlockscreen -u path/to/lockscreen/wallpaper.jpg
```

Add this to `/etc/environment`
```
XDG_CURRENT_DESKTOP=Unity
QT_QPA_PLATFORMTHEME=gtk2
```

#### Copying all the config files

1) Copy `bspwmrc` to `~/.config/bspwm/bspwmrc`
2) Copy `bashrc` to `~/.bashrc`
3) Copy `polybar-config` to `~/.config/polybar/config`
4) Copy `polybarlaunch.sh` as a startup logic to `~/.config/polybar/polybarlauch.sh`
5) Copy `awesome.rasi` to `~/.config/rofi/awesome.rasi`
6) copy `config.rasi` to `~/.config/rofi/config.rasi`
7) Copy `picom.conf` to `~/.config/picom/picom.conf` (optional)
8) If you want my edited `sxhkdrc` config, copy `sxhkdrc` to`~/.config/sxhkd/sxhkdrc`

The cheater method (Assuming you cloned all the files in the home directory):
```
cp ~/shua-bspwm/bashrc ~/.bashrc && cp ~/shua-bspwm/bspwmrc ~/.config/bspwm/bspwmrc && cp ~/shua-bspwm/polybar-config ~/.config/polybar/config && cp ~/shua-bspwm/polybarlauch.sh ~/.config/polybar/polybarlauch.sh && cp ~/shua-bspwm/awesome.rasi ~/.config/rofi/awesome.rasi && cp ~/shua-bspwm/config.rasi ~/.config/picom/config.rasi && cp ~/shua-bspwm/picom.conf ~/.config/picom.picom.conf && cp ~/bspwm-shua/sxhkdrc ~/.config/sxhkd/sxhkdrc
```

Note: the `source .bashrc` command is not yet executed unless you're done setting up bspwm because neofetch can slightly slow down your PC.

# Finishing commands

1) Match the terminal and CLI text editor color scheme with wallpaper using wal:
```
wal -i path/to/your/wallpaper.png
```
Usually the folder for your wallpapers are in `/usr/share/backgrounds/` directory.

2) Sourcing `.bashrc`
```
source .bashrc
```
3) Restart bspwm by pressing `super + alt + R` (assuming you haven't edited `sxhkdrc` yet before switching to bspwm).
4) Done.

Icons:
1) Neonyt-Dark-Icons https://www.gnome-look.org/s/Gnome/p/1463720
2) Win7Build-dark-cursors https://www.gnome-look.org/p/1437431/

#### Program list

1) Picom, as a compositing manager.
2) Nitrogen, a wallpaper manager.
3) GNOME Screenshot, a GNOME screenshot utility.
4) Pywal, a color scheme generator.
5) LXSession, a polkit from the LXDE Desktop Environment.
6) Roboto, a mono-style font.
7) LXAppearance, a theme customizer from the LXDE Desktop Environment.
8) GNOME Materia Theme, a pack of GNOME Materia themes to customize your desktop theme.
9) Betterlockscreen, a simple lockscreen to setup.
10) Sakura, a customizable terminal emulator.
