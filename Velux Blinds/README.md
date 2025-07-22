I searched the Internet for a way to control my Velux blinds, but could only find very simple, relay-based ways to control the remote.
The remote in question is the KLI 312 (BG-RCO11-02)
The soulutions I found were too complicated, using relays and also needed a bunch of passive components to make it all work.
They were also only targeting the Up/Stop/Down functions of the remote.

I figured I could try to make a more sleaker and simpler way of controling the remote.
Using an ESP-module (ESP-12e) I had laying around, I was able to access all functions of the remote!
The goal was also to have it integrated into Home Assistant.

This is the result!

I am using a ESP-12e, but other ESP-modules could also be used.
What's important are the available GPIO-pins.
In this case 5 GPIO-pins are used: GPIO4, GPIO5, GPIO12, GPIO13 and GPIO16.
The ESP also need to be enabled, which is done by connecting the ENABLE-pin to VCC.

I programmed the ESP-module with a basic-configuration before soldering it to the remote, using ESPHome's web-based upload tool.
https://web.esphome.io/?dashboard_wizard
Configurations like connecting to WiFi will not be covered here.

Good luck!
