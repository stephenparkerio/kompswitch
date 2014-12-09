KompSwitch
==========

KompSwitch corrects the flickering DVD playback on some Ubuntu systems with compositing enabled.

### Install ###
1. Open up Terminal (or any command line interface) Applications > Accessories > Terminal
2. Download the installer

		wget https://github.com/withaspark/kompswitch/kompswitch.install

3. Make the installer executable 

		chmod u+x kompswitch.install

4. Run the installation script 

		~/kompswitch.install --auto
 (if you want to choose the DVD player yourself, do not include the --auto part).

5. Done! There is now an icon on your Desktop called KompSwitch Play DVD.

If you don't want an icon or prefer the command line, you can also run KompSwitch with
```sh
~/kompswitch [--player PLAYER]
```

Include the --player option if you want to explicitly set which DVD player to use, such as totem, vlc, etc.

Hope it helps you Ubuntu/Kubuntu/Xubuntu users.

### Customize ###

You can give the installer a cool icon by right clicking the desktop icon, clicking the spring board icon, and selecting a suitable image.

If you like a clean desktop, you can always add the desktop launcher to your panel by dragging the desktop launcher onto it and deleting the desktop one.

### Uninstallation ###
If for any reason you should choose to remove kompswitch, a complete removal can be invoked by
```sh
~/kompswitch --uninstall
```

### Further Consideration ###
If you are having the same problem in Kubuntu or Xubuntu, you will have to change the ```MAIN_DE``` and ```TEMP_DE``` values to whichever applies to your flavor of Ubuntu.

If your DVD drive can not be found from /dev/dvd, you will have to change the ```DVD_DRIVE``` value to the location of your drive.

Both of these can easily be changed by editing the top few lines in the script.

```sh
vim ~/kompswitch
```

If you're having any problems, just contact me via a GitHub issue on this repo or my website https://withaspark.com.
