# Raspberry Pi0W with adafruit mini pitft (Mini-PiTFT, MiniPiTFT or MPiTFT) rgb display 1.14" 240x135 st7789 (2 tactile buttons (programmed))

Install raspbian lite (Bullseye -latest as of this creation) to sd media with raspberry pi imager.

Install Pi Hole

Use the following instructions to install Pi Hole:

https://github.com/pi-hole/pi-hole/#one-step-automated-install

Original code is from Adafruit's Pi Hole Ad Blocker with Pi Zero W guide. Follow this guide to install the mpitft.

https://learn.adafruit.com/pi-hole-ad-blocker-with-pi-zero-w?view=all#install-mini-pitft

To install the library for the Pi OLED, enter the following into the terminal:

sudo apt-get install python3-pip
sudo pip3 install adafruit-circuitpython-ssd1306

We also need PIL to allow using text with custom fonts. There are several system libraries that PIL relies on, so installing via a package manager is the easiest way to bring in everything:

sudo apt-get install python3-pil

And let's also make sure the requests module is installed:

sudo pip3 install requests

# Skip to Install Mini PiTFT at this point, do not continue with OLED portion.

We've updated our popular PiOLED script for use with the Mini PiTFT, a 135x240 Color TFT add-on for your Raspberry Pi. This cute little display has two tactile buttons on GPIO pins that we'll use to make a simple user-interface display for your Pi-Hole.

If you are getting a ModuleNotFound error, you may need to install the Python libraries by prepending the sudo command before the pip command since you will need to run the script as sudo.

Instead of using the stats.py file they suggest at this point, use the included clock.py of this repository.

![IMG_0388](https://user-images.githubusercontent.com/98209729/160754380-33160d1a-0b94-4b92-9e84-cf10d2a3b15e.jpeg)
![IMG_0393](https://user-images.githubusercontent.com/98209729/160754430-9cccee92-ea79-4d8f-a115-864affa8b315.jpeg)
![IMG_0394](https://user-images.githubusercontent.com/98209729/160754491-85814b54-980c-465a-9b54-a454f53241ce.jpeg)



