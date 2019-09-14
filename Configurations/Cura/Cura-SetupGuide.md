# Cura v.15.x Setup Guide for Prusa i3 - TRONXY P802D

Download Cura 15.x for your computer:

* Mac - [v15.04.6](http://software.ultimaker.com/current/Cura-15.04.6-MacOS.dmg)
* Windows [v15.02.1](https://cura1.software.informer.com/15.0/)

I've found better luck with the older version of Cura but encourage you to check out newer versions to suit your needs.

This tutorial is based off of the 15.x version but once you undersand the basics, you should be able to configure the newer versions.

1. Add a new Machine
    * This happens by default if this is the first time you ever ran Cura, otherwise "Add new machine" is found in the "Machine" menu.
    * Just click "Next"

![Setup 1](/Files/cura1.png)

2. Select your Machine
    * Select the last choice: "Other"

![Setup 1](/Files/cura2.png)

3. Other machine information
    * You may not see this screen depending on your version of Cura
    * Just click "Next" with nothing selected

![Setup 1](/Files/cura3.png)

4. Custom RepRap information
  * Here is where you enter your machine specific information
    * Machine Name: You pick a name
    * Machine width X (mm): 220
    * Machine width Y (mm): 220
    * Machine width Z (mm): 180
    * Nozzle size (mm): 0.4
    * Heated bed: Yes (check)
    * Bed center is 0,0,0 (RoStock): No

![Setup 1](/Files/cura4.png)

5. After Setup you will be dropped into the application, this is the view you will see when you launch from now on. *Each entry has help if you mouse over.

5a. If you planning on running your printer from your computer vs. SD card you may need to check the port and baud rate. Machine settings is accessible from the top menu.

On a Mac it will look like this:

![Setup 1](/Files/machine_settings.png)

Port will vary but baud rate should be 115200

6. There are a few settings to check on the "Basic" screen
  * Layer height - this refers to the quality of your print.
      * 0.1 is very fine/high quality - long print time
      * 0.3 is course, good for sturuture over beauty - faster
  * Shell thickness - this is how many layers to print the outer wall thickness. It needs to be a multiplier of the nozzel size (0.4)
      * 0.4 - very thin, single layer
      * 0.8 - 2x - good start for most prints
      * 1.2+ - 3x+ - stronger outside walls

  * Fill Density - how much fill/how solid to make the print. 0-100% - Unless you need very strong/dense prints start at 10-20%.

  * Print speed - you will tweak this with experience and based on the print. The slower the higher the quality/fine detail. For low detail prints you can increase it. 30mm/s will give better/best quality but longer time.

  * Print Temperature is the melting point of your filament, 210-220 for PLA, 230-250 for ABS, check the vendor's recommendations or do test prints to determine what is best for the filament being used.

  * Bed temperature is the temperature of the heated surface you are printing onto. Not all plastics require a heated bed, PLA it is optional. It helps in reducing warping of the printed material. Refer to filament for settings. Setting to 0 will disable heated bed.

  * Diameter - you will need to check this as by default it is not correct, the correct setting for your printer will always be 1.75mm.

  * Nozzle size - this should have been carried over from setup, but check to verify, it should be 0.4. This could change if you buy and install different nozzels.

![Setup 1](/Files/cura5.png)

7. "Advanced" screen - this includes settings relative to speed and quality fine tuning
  * Retraction - this is the extruder setting to retract filament so it doesn't leave "stringy" lines on your print
    * Speed of 40.0 and distance of 6mm is a good start
  * Speed has an impact on quality, default settings are a good place to start, experience may have you change it to suit the print. The remaining fields that have 0.0 will take the system wide speed setting, otherwise a non-zero entry will override the speed set on the "Basic" page.

![Setup 1](/Files/cura6.png)



