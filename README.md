> [!WARNING]
I recommend using this script on a Virtual Machine with at least 30 GIO, just to be safe. Also the script will disable passwords on the system and it will not create the ISO, just configure it and install some utility tool to do it. This script is only for linux mint cinnamon system.

For these script I recommend the use of virtual machines, you can use [VirtualBox](https://www.virtualbox.org/wiki/Downloads) or Virt-Manager. 

These scripts are a starting point to create a toolbox system which can be export as an ISO. The objectives of these scripts are to create an all-in-one liveUSB system who can repair,backup or customize your computer if you need it.

# Installation 

Run the following command in the terminal 
```
./Install
```
Then after the reboot, run the following command again in the terminal:

```
./After_show
```

The Install script will install some utility tool to the system and remove unecessary softwares, it will also configure the system to run rootless and when the script is finished, it will reboot your system.

The After_show script will install [penguins-eggs](https://penguins-eggs.net/) and remove the folder.

Penguin-eggs is a console utility that allows you to remaster your system and redistribute it as iso images, there is a lot of option with this tool but for the live system, we will simply use : 

```
sudo eggs produce --clone
```
> [!TIP]
You can even add the option --max for maximum compression when you are finished customizing and testing the system. 

The console utilty will ask with a `no` or `yes`, just answers with `no`, then it will ask the permission to use the storage to create the ISO, choose `yes`.

The ISO will be located in `/home/eggs/.mnt/`

Here is a list of the themes installed :

Cursor = oreo_spark_purple_cursors from (https://github.com/milkmadedev/oreo-cursors-compiled) 

Icon-themes = Tela-green from (https://github.com/vinceliuice/Tela-icon-theme.git)

Gtk-themes= Vimix-dark-doder from (https://github.com/vinceliuice/Vimix-gtk-themes.git)

Plymouth=linux_mac_style from (https://www.gnome-look.org/p/2106821)
