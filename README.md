# TallyArbiter-M5AtomMatrixListener
This is my continued attempt at 'mushing' arduino code.
This is a Tally Viewer using a M5 Atom Matrix as a TallyArbiter Client.
To learn more about the Tally Arbiter project, [click here](http://github.com/josephdadams/tallyarbiter).

You can buy an M5 ATOM Matrix here:
https://m5stack.com/collections/m5-atom/products/atom-matrix-esp32-development-kit
OR
https://www.adafruit.com/product/4497 (Shipped from USA)

# Instructions 
This is the slower (but seems to always work) way:

1. Download the .bin file here - https://github.com/themusicnerd/TallyArbiter-M5AtomMatrixListener/blob/main/tallyarbiter-m5atom.bin
2. Download ESPHomeFlasher here - https://github.com/esphome/esphome-flasher/releases/tag/1.4.0
3. Connect your M5-Atom to your computer using a USB cable
4. Open ESPHome Flasher
5. Select your M5-Atom (USB Serial Port) - Usually COM3
6. Click Browse
7. Find and Select the .bin file
8. Click "Flash ESP"
9. WAIT for Configuration installed! (takes about 90 seconds)
10. Within 2 min on boot - get a wifi device and connect to the m5atom-XXXXX wifi network (note the XXXXXX for later)
11. Wait for captive portal or goto 192.168.4.1
12. Click "Setup"
13. Enter Tally Arbiter Server IP Address
14. Check Tally Arbiter Port is correct (Defulat 4455)
15. Click Save
16. Renavigate to 192.168.4.1
17. Click Configure WiFi
18. WAIT while is scans wifi networks
19. Configure Wifi
20. Wait for green tick
21. Press screen (which is a button) to set the number on the local screen only
22. Assign unit in Tally Arbiter under Settings > Listeners > m5Atom-XXXXXX

## Troubleshooting

### macOS
If you receive an error similar to `ImportError: No module named serial` reference: https://community.m5stack.com/post/11106

# Videos

* What this does when used with TallyArbiter - https://youtu.be/hNhU22OkXek
* Demo of the M5Atom Matrix code in this git - https://youtu.be/Mc_PCxg6qdc
* Demo running on 10 M5Atom Matrix units via a cloud server - https://youtu.be/TiqjmXdzPic

# Current Updates
* Tidyed up things a little bit
* Changed the way the LED's are written to now using the M5 library
* Added Blank and 1 thru 16 camera numbers by pushing the screen (M5 Action button)
* Fixed bugs

Note if deploying yourself, one of the librarys has an error where you have to manually comment out hexdump by changing it to //hexdump

# Planned Updates
Next Update will have Internal Motion Unit functionality to automatically rotate the screen.

# Thanks
Thanks to mg-1999 for the code base, and huge thanks to josephdadams for his amazing work on TallyArbiter, and the origional M5StickC implementation.
https://github.com/josephdadams/TallyArbiter
