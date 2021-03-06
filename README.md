# shua-bspwm
A custom bspwm theme for beginners.

First, clone the git repository.
```
git clone https://github.com/Shua24/shua-bspwm.git
```
# Setting up bspwm

Before copying the config files, install the dependencies first.
#### Arch-based distros:
If you use paru:
```
paru -S bspwm rofi polybar lxsession picom nitrogen pywal ttf-roboto qt5-styleplugins lxappearance materia-gtk-theme -y
```
If you're using yay:
```
yay -S bspwm rofi polybar lxsession picom nitrogen pywal ttf-roboto qt5-styleplugins lxappearance materia-gtk-theme -y
```
(You can also edit the bspwm keybinds in `~/.config/sxhkd/sxhkdrc` before switching to bspwm to add a keybind for `rofi` and other programs)

Before you copy all the icons and config files, set the terminal font to Roboto Mono.

#### Copying the icons
1) Extract all icons.
2) Copy `Win7Build-dark-cursors` and `Neonyt-Dark-Icons` into the `~/.icons` directory.

The cheater method (Assuming you cloned all the config files in the home directory):
```
cp ~/shua-bspwm/Neonyt-Dark-Icons/ ~/.icons/Cyan-Breeze-Dark-Icons/
cp ~/shua-bspwm/Win7Bulid-dark-cursors/ ~/.icons/Win7Bulid-dark-cursors/
```
Before you copy the config files, setup the dark theme and icons by opening `lxappearance`. Don't forget to setup a wallpaper using `nitrogen` by adding a directory to the preferences.

#### Copying all the config files

1) Copy `bspwmrc` to `~/.config/bspwm/bspwmrc`
2) Copy `bashrc` to `~/.bashrc`
3) Copy `polybar-config` to `~/.config/polybar/config`
4) Copy `polybarlaunch.sh` as a startup logic to `~/.config/polybar/polybarlauch.sh`
5) Set a permission to execute the script
```
chmod +x ~/.config/polybar/polybarlaunch.sh
```
6) Copy `picom.conf` to `~/.config/picom/picom.conf` (optional)

The cheater method (Assuming you cloned all the files in the home directory):
```
cp ~/shua-bspwm/bashrc ~/.bashrc
cp ~/shua-bspwm/bspwmrc ~/.config/bspwm/bspwmrc
cp ~/shua-bspwm/polybar-config ~/.config/polybar/config
cp ~/shua-bspwm/polybarlauch.sh ~/.config/polybar/polybarlauch.sh
cp ~/shua-bspwm/picom.conf ~/.config/picom.picom.conf
```

Note: the `source .bashrc` command is not yet executed unless you're done setting up bspwm because neofetch can slightly slow down your PC.

# Finishing commands

1) Match the terminal and CLI text editor color scheme with wallpaper using wal:
```
wal -i path/to/your/wallpaper.png
```
Usually the folder for your wallpapers is in `/usr/share/backgrounds/` directory.

2) Sourcing `.bashrc`
```
source .bashrc
```
If you have multiple desktop environments, you can add the `-n` flag to the `wal` command in `.bashrc`.

3) Restart bspwm by pressing `super + alt + R` (assuming you haven't edited `sxhkdrc` yet).
4) Done.

Note that this is only the basic setup for my bspwm config. If you want to turn my setup into a desktop environment, see the full branch of this repository.

Icons:
1) Neonyt-Dark-Icons https://www.gnome-look.org/s/Gnome/p/1463720
2) Win7Build-dark-cursors https://www.gnome-look.org/p/1437431/

Note that the font I'm using is Flexi IBM VGA False, you can setup the fonts yourself by installing Flexi IBM VGA False from dafont.com.
