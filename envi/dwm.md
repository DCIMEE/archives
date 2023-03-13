### Pre-requisites

- xorg-server 
- xorg-xinit 
- libx11 
- libxinerama 
- libxft 
- webkit2gtk  


### First
git clone http://git.suckless.org/dwm, st, dmenu, slstatus  

add `exec dwm` on *"~/.xinitrc"*  

type command below to open dwm  

`startx / sudo startx`  

### Changes
To make changes works  
```bash  
rm config.h  
```
 edit **config.def.h**  

```bash
sudo make clean install  
```
restart the specific program.  

### Patches
Download the diff file to the root directory of *"dwm/st/.."*
use below command to patch.  
`patch < 'patch name'`  
Recompile and restart.   

### Autostart (patch)
after intall  
`mkdir ~/.dwm`  
make a file "autostart.sh" under *"~/.dwm"*  
add **"#!/usr/bin/env bash"** on the first line  
After changes, run `sudo chmod +x autostart.sh` to make it exectueable  

add `exec slstatus &` for example in "autostart.sh"  

" **xwallpaper**
get one wallpaper  
`"xwallerpaper --zoom ~/.Download/wall.png` add on "autostart.sh"  


#### Optional Fonts (icons)
to show icons  
package name : ttf-nerd-fonts-symbols  
