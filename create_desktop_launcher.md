It would be easier if we can have a simple desktop launcher instead of entering a range of terminal commands . 

This will provide the set of instructions to create a desktop laucher that enables you to directly access label-studio with just a click !

## Resources 
```
https://linuxconfig.org/how-to-create-desktop-shortcut-launcher-on-ubuntu-18-04-bionic-beaver-linux
https://askubuntu.com/questions/182700/desktop-shortcut-for-terminal-command
```
## Steps

Step 01 : Create a .desktop file 
Requirements : 
a) logo , set of commands to be entered in the terminal 
```
gedit ~/Desktop/LabelStudio.desktop
```

Step02 : Once the gedit editor opens , paste the following code there as save it . Make sure you have the logo file in the same path or else please edit the Icon field . 
```
#!/usr/bin/env xdg-open
[Desktop Entry]
Version=1.0
Type=Application
Terminal=false
Exec=sh -c "export LABEL_STUDIO_LOCAL_FILES_SERVING_ENABLED=true ;label-studio start"
Name=label-studio
Comment=label-studio
Icon = /home/surya/Desktop/label-studio/logo.png
```

This creates a .desktop file on your desktop , click on it . If it prompts the following error : 
```
The application launcher "Skype.dekstop" has not been marked as trusted.
If you do not know the source of this file, launching it may be unsafe.
```

Then ....

Step 03 : 
Properties-->Permissions-->Allow executing file as program.
