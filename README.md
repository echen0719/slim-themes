# Cool SLiM Themes

I installed and use Linux (Arch BTW) as my operating on a daily basis. I could use CLI but I do want a good-looking, simple, memory efficent display manager that greets meet on startup and locks my screen when I am away. Here are some of my SLiM themes to share.

**About Slim:** SLiM stands for "Simple Login Manager". It uses low amounts of resources and is highly customizable, perfect for many systems. However, SLiM is outdated with last update to it being in 2013. There might be better options that I might look into the future, but SLiM works perfectly fine for me. 

## Installation

1. According to your Linux distro, find the SLiM package in repositories.
2. Install SLiM using distro package manager.

Debian based systems:
```sh
$ sudo apt-get install slim
```
Fedora based systems:
```sh
$ sudo dnf install slim
```
Arch based systems:
```
$ sudo pacman -S slim
```

3. Enable SLiM if needed (i.e. systemd).

## SLiM Theme Configuration

1. You can browse the Github repository to download all SLiM themes. You can choose multiple at the same time.
2. After SLiM is installed, theme folders should be located at /usr/share/slim/themes/. Check this directory to make sure they are there.
3. Copy and paste or move the **folder** of the theme that you have downloaded into this folder.
4. Use your system editor to edit /etc/slim.conf and there should be a value called **current_theme** towards the bottom.

Change the value to the name of the theme folder your choose: 

```sh
# current theme, use comma separated list to specify a set to
# randomly choose from
current_theme       Arch Dark Text
```

If you use xorg/xinit for your display, make sure you find and change the value **login_cmd** to your xinit file location.

```sh
# NOTE: if your system does not have bash you need to adjust the command
# according to your preferred shell, e.g. for freebsd use:
# login_cmd         exec /bin/sh - ~/.xinitrc %session
login_cmd           exec /bin/bash -login /etc/X11/xinit/xinitrc
```

5. Reboot your system and enjoy your new SLiM theme!

## Future

I am going to continue to make SLiM themes but I also have school. I'll try my best to add more themes for you guys.

## Why SLiM?

I know that SLiM has basically been dead for the past decade. I use it because it is just efficent, low memory usage, and is perfectly customizable. Sometimes, things don't need to be frequently updated for it to work.

*** Note: The Arch Linux Wiki has a great page on SLiM: https://wiki.archlinux.org/title/SLiM.
