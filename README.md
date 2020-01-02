Pithosfly
------

A fork for Pithos, a native Pandora Radio client for Linux, that saves the stream you are listening to disk.
It downloads, rips music intelligently, saving songs into mp3 files into individual folders, named after a radio stream. The files are properly tagged and the cover art is saved into the mp3.

Configure folder to save to by adding the following to pithos.ini (usually found in ~/.config/):

`save_to=/path/to/folder`

Run:

`cd /folder/with/source`

`python3 -m pithos`

Or to see verbose output run

`python3 -m pithos -v`

You can also build and install per Pithos' own instructions:
* Remove if already installed installed
* Get the prerequisites
```
sudo apt-get install python3-setuptools python3-dbus python3-gi python3-gi-cairo \
  gir1.2-gstreamer-1.0 gir1.2-gst-plugins-base-1.0 gstreamer1.0-plugins-good gstreamer1.0-plugins-bad  \
  python3-pylast gir1.2-appindicator3-0.1 gir1.2-notify-0.7 gir1.2-keybinder-3.0 gnome-icon-theme-symbolic \
  python3-mutagen
```

Note: that python3-mutagen is available for Ubuntu 15.10 and after, however it works fine on earlier releases. You can get it from [here](https://launchpad.net/ubuntu/+source/mutagen).

* Then run

`sudo ./setup.py install`

(you might need some more libs for the latest pithos). More details [here](https://github.com/pithos/pithos/wiki/Installing-from-Source).

The original Pithos [homepage is here](http://pithos.github.io).

This fork follows the mainline code commits.

License: GNU GPLv3
