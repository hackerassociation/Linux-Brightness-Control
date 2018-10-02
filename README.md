{% seo %}
google-site-verification: googlef9ae6d76a25515b6.html
# Welcome to the Linux-Brightness-Control Page!
Cannot change brightness? or brightness control not working?<br>Take a look at brightness-controller version 1!<br>
![screenshot](https://github.com/hackerassociation/Linux-Brightness-Control/blob/master/at%2078.png)

## Prerequisites and Installation
**1. Check if you are intel, if yes, perform below** [[7]](https://itsfoss.com/fix-brightness-ubuntu-1310/)
* `ls /sys/class/backlight/`
* `sudo touch /usr/share/X11/xorg.conf.d/20-intel.conf`
* `sudo gedit /usr/share/X11/xorg.conf.d/20-intel.conf`
>       Section Device
>       Identifier  "card0"
>       Driver      "intel"
>       Option      "Backlight"  "intel_backlight"
>       BusID       "PCI:0:2:0"
>       EndSection`
* `sudo reboot`<br >

**2. Download the python script "Brightness"** [[2-4]](https://www.youtube.com/watch?v=JadLzxetiqY)<br >
**3. Run the following commands in the command prompt** 
* `sudo apt-get install xbacklight` 
* `sudo apt-get install python3-tk` 
* `chmod +x brightness-control`

**4. Change the settings of nautilus to ask each time on executable** [[1]](https://askubuntu.com/questions/761365/how-to-run-a-python-program-directly)<br >
**5. Double click on the "brightness-control" python program to control brightness!**

### References
1. https://askubuntu.com/questions/761365/how-to-run-a-python-program-directly
2. https://www.youtube.com/watch?v=JadLzxetiqY
3. https://stackoverflow.com/questions/14508727/how-to-get-value-out-from-the-tkinter-slider-scale 
4. https://docs.python.org/3/library/subprocess.html#subprocess.run
5. https://itsfoss.com/fix-brightness-ubuntu-1310/

By: HackerAssociation
