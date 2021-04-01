# i3_Ricing

This is the repository containig the ricibg configuration of the system. Please follow the steps of the README.md file in the repository to get the desired effect of ricing. 

i3 is one of the most popular open source software that is used for ricing. 'Ricing' basically represents customizing desktop and enables multi-tasking tiling features and so on.

## To install

``` bash
$ sudo apt install i3
$ sudo apt install feh thunar rofi pavucontrol arandr i3blocks compton lxappearance
```
Logout of the window and on the login screen, you will get a white icon depicting the i3 window manager, select that and login.

#### On login, you will get to choose _Win_ or _Alt_ keys to be your Mod key. It is preferable to use the _Win_ key but you can use the _Alt_ key as well.

Now, you are good to go. 
#### Patch the i3 folder from the repository and place it in your _.config_ folder of your _home_ directory.

Please note that _.config_ is a hidden folder. 

## Basic key bindings

#### Win + Enter => Opens the Terminal
#### Win + Shift + Q => Terminates the ongoing process upon which the cursor is hovering
#### Win + D => Opens the DMenu (An application where you can search for installed applications)
#### Win + H => It causes horizontal tiling. Press the keys simultanoeusly and open a new window. It gets added to the side of the existing window.
#### Win + V => It causes vertical tiling. Press the keys simultanoeusly and open a new window. It gets added to the bottom of the existing window.
#### Win + Up Arrow Key or Win + L => Shifts the focus to the window above the current window. (Applicable only when vertical tiling is done)
#### Win + Down Arrow Key or Win + K => Shifts the focus to the window below the current window. (Applicable only when vertical tiling is done)
#### Win + Left Arrow Key or Win + J => Shifts the focus to the window to the left of the current window. (Applicable only when horizontal tiling is done)
#### Win + Right Arrow Key or Win + ; => Shifts the focus to the window to the right of the current window. (Applicable only when horizontal tiling is done)
#### Win + S => Stacks the windows.
#### Win + E => Tiles the windows.
#### Win + W => Toggles the windows.
#### Win + F => Changes to Fullscreen mode.
#### Win + Shift + C => Reloads the current windows.
#### Win + R => Activates the resize mode. Hover over the window you want to resize and use the arrow keys to resize the windows.
#### Win + Shift + R => Restarts the i3 manager.
#### Win + Shift + Space => Floats the window and makes it draggable.
#### Win + Shift + X => Locks the screen.
#### Win + Num (1 to 0) => Opens a workspace numbered 1 to 0 
#### Win + Shift + Num (1 to 0) => Shifts the window upon which it is hovered to the workspace numbered 1 to 0
#### Win + Shift + E => Logout of i3.

These key bindings can be altered in the _config_ file of i3.

## Customizing Wallpaper and Resolution

#### Please change the directory to the images file given in Line 206 and 227 of config file to the image location of your respective wallpaper and lockscreen.
#### Lockscreen only supports _.png_ files

``` bash
$ xrandr
```
Copy the output and paste it in line 228 followed by exec_always. It sets the resolution of your screen and it helps in adjusting multiple monitors.

## Renaming Workspaces and Assigning Applications

#### Workspaces can be renamed by assigning names within the inverted commas in the lines 108 to 117 of the config file.
#### Applications can be assigned by using the xprop command and making subsequent changes in the config files 

``` bash
$ xprop
```
Click on the application and get the class and assign it using the syntax in line 131.

## Opening Applications on Boot

#### Use the exec_always line in the code of the _config_ file. Example shown in line 224 and 225.  

## Downloading Fonts 

#### You can download fonts and install them. For example, I have installed the [Yosemite San Francisco Font](https://github.com/supermarin/YosemiteSanFranciscoFont) in my system. 
#### Download the font in .zip format from the link in _Manual Install_ section of the repository.

``` bash
$ cd Downloads 
$ unzip YosemiteSanFranciscoFont-master.zip
$ cd YosemiteSanFranciscoFont-master 
$ mv *.ttf ~/.fonts/
```

You can now see the font already installed in lxappearance as 'SFNS Display'. Adjust the font size also. Change line 16 of config file as well to apply the font to all sectors.

## Changing colour of the bar and windows

#### You can change the colours of the windows (both activa and inactive) by inserting hexadecimal colours in line 179 to 184.
#### You can also customize the bar by i3blocks (discussed later).

## Installing icons and theme

#### You can install icon packs and themes and implement them in your system using lxappearance.
#### Suggested sites for downloading iconpacks are:

* [Pling-store](https://www.pling.com/)
* [Gnome-Look](https://www.gnome-look.org/browse/cat/)























