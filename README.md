# retroscreensavers
My collection of retro screensavers can be found [here](https://drive.google.com/open?id=1JghlJYllOwpC7O6MA-K1OJQ3gIyenS2_)
# Dependencies
* coreutils
* mpv
* xscreensaver
# Installation
## Ubuntu/Mint (the only distros I've tested)
1. You should be able to install the dependencies and extra screensavers for xscreensaver at once.
```
sudo apt-get install xscreensaver xscreensaver-gl-extra xscreensaver-data-extra coreutils mpv
```
2. Open `retro` in your choice of text editor and pay attention to my comments starting with "#" there are values that can be
edited like the path of the videos, what will play during the day or night, and what time day or night starts. These are really
the only things you need to edit, the other lines serve to make sure `mpv` closes correctly and videos aren't repeated
so tweak at your own discretion.
3. Then `cd` to the directory of the downloaded `retro` script, make it executable, and send it to usr/lib/xscreensavers with: 
```
sudo cp retro /usr/lib/xscreensaver/retro && sudo chmod +x /usr/lib/xscreensaver/retro
```
4. Initialize xscreensaver by searching your programs and opening it, or with `xscreensaver-demo` in a terminal. 
You should be able to see a lot of screensavers and various settings you can tweak.
5. Finally, after opening xscreensaver a file (.xscreensaver) will be autopmatically created in your home directory.
Edit  .xscreensaver in your choice of text editor to include this line within the "programs" category 
under all the other various screensavers.:
```
GL:   retro retro     \n\
```
6. Open xscreensaver back up and scroll down to select the Retro screensaver. 
If configured correctly, you should see your videos after clicking Preview!

# Other Distros
xscreensavers should be installable across most distros, check your repos for more info. 
After it's installed, it should be a whole lot different than the above instructions, make sure videos and script is in the
right place.

Contributors
------------------------
* thegriffindude
* [graysky2](https://github.com/graysky2) The script is basically just his for Apple Aerial Wallpapers, just tweaked.
