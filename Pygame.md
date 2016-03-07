Pygame also comes with [Raspbian](https://github.com/project-owner/Peppy.doc/wiki/Raspbian). To make sure that it's really there start [Python](https://github.com/project-owner/Peppy.doc/wiki/Python) interpreter and type the following line at prompt:
```python
import pygame
```
You shouldn't see any exceptions. If you'll see import exception that means there is no Pygame and it should be downloaded and installed from their [web site](http://www.pygame.org/download.shtml).

The [Raspbian Jessie](https://github.com/project-owner/Peppy.doc/wiki/Raspbian) has some incompatibility issues with SDL 2.x used by Pygame. That makes the [touchscreen](https://github.com/project-owner/Peppy.doc/wiki/Touchscreen) unusable. The workaround is to get SDL 1.2 from the previous Raspbian version - Wheezy. How to do that was explained [here](https://learn.adafruit.com/adafruit-2-4-pitft-hat-with-resistive-touchscreen-mini-kit/pitft-pygame-tips).

Create the script [installsdl.sh](https://github.com/project-owner/Peppy.doc/blob/master/files/installsdl.sh) and run it:
```
sudo chmod +x installsdl.sh
sudo ./installsdl.sh
```
After this step the [touchscreen](https://github.com/project-owner/Peppy.doc/wiki/Python) should start working properly with Pygame library.

[<<Previous](https://github.com/project-owner/Peppy.doc/wiki/Python) | [Next>>](https://github.com/project-owner/Peppy.doc/wiki/Mpd & Mpc)