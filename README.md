# Some SLiM Themes

I installed and use Linux (Arch BTW) as my operating on a daily basis. I could use CLI but I do want a good-looking, simple, memory efficent display manager that greets meet on startup and locks my screen when I am away. Here are some of my SLiM themes to share.

## Installion

1. According to your Linux distro, find the SLiM package in their repositories.
2. Install SLiM using distro package manager.

Debian Based: sudo apt-get install slim
Fedora Based: sudo dnf install slim
Arch Based: sudo pacman -S slim

## SLiM Theme Configuration

1. You can go to releases to download all SLiM themes if you want or you can download each individual folder yourself
2. After SLiM is installed, theme folders should be located at /usr/share/slim/themes/. Check this directory to make sure they are there
3. Copy and paste or move the folder of the theme that you have downloaded into this folder
4. Use your system editor to edit /etc/slim.conf and change the value of current theme to the theme's folder name (i.e. Arch Dark Text)

If you use xorg for your display, make sure you find and change the value of your xinit config file (i.e. exec /bin/bash -login /etc/X11/xinit/xinitrc %session)

5. Reboot your system if nessecary and enjoy your SLiM themes

## Future

I am going to continue to make SLiM themes but I also have school. I'll try to add at least a few per month. 

## Why SLiM?

I know that SLiM has basically been dead for the past decade. I use it because it is just efficent, low memory usage, and is perfectly customizable. Sometimes, things don't need to be frequently updated for it to work.
