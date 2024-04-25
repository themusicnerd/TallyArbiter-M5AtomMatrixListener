# TallyArbiter-M5AtomMatrixListener
This is my continued attempt at 'mushing' arduino code.
This is a Tally Viewer using a M5 Atom Matrix as a TallyArbiter Client.
To learn more about the Tally Arbiter project, [click here](http://github.com/josephdadams/tallyarbiter).

You can buy an M5 ATOM Matrix here:
https://m5stack.com/collections/m5-atom/products/atom-matrix-esp32-development-kit
OR
https://www.adafruit.com/product/4497 (Shipped from USA)

# Instructions

1. Download the .bin file here - 
2. Connect your M5-Atom to your computer using a USB cable
3. Go to https://web.esphome.io/
4. Click "Connect"
5. Select your M5-Atom (USB Serial Port) - Usually COM3
6. Click "Connect"
7. Click "Install"
8. Click "Choose File"
9. Find and Select the .bin file
10. Click "INSTALL"
11. WAIT!
12. 

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
