<h1>Laterna Stick</h1>

Laterna Stick is the plugable version of our [Laterna RGB Controller](https://github.com/monoapp3/Laterna.git "Laterna's Homepage"). You can use this board for small projects, where not more than a LED Strip channel is required. Besides the LED Strip Channel, the board provides some IO Pins which can be used with sensors and buttons if required by your project.You can power the board using the USB Type A connector or using an external 5V power supply. Please refer to power consumption section for more details. (**Work in Progress**)

The Laterna series of boards are mainly intended to be used with [WLED software ](https://github.com/Aircoookie/WLED "WLED's Homepage") or [ESPHome](https://esphome.io), but you can also program the board using your own code or other library.

The controller can be ordered on [Aliexpress](https://www.aliexpress.com/item/1005003777511039.html?spm=5261.ProductManageOnline.0.0.3aaa4edfzpZkav)<br>

<h3>Features</h3>
Chip:   ESP32 WROOM 32E Wifi and Bluetooth
<br>USB Type A connector for flashing and 5V power
<br>CP2102 USB to serial chip for easy flashing (https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers) 
<br>1 channel for adressable LED strip with 3 or 4 pins (e.g. WS281x, WS2801, SK6812 etc.)
<br>3A resettable Fuse (https://en.wikipedia.org/wiki/Resettable_fuse)
<br>5V VIN

<img src="/Photos/Stick2.png" width="50%">

<h3>Installation</h3>

All our boards are delivered with a default WLED version **link to board version and software flashed**.You can use the board out of the box after you solder required connectors.

You can customize the software based on your needs and flash it by **USB** or the **programming connector**.
The board has an integrated CP2102 USB to UART bridge so you can flash it without using **any additional hardware**.

For Flashing a precompiled Firmware we recommend [ESPHome Flasher](https://github.com/esphome/esphome-flasher/releases "ESPHome Flasher Releases")

We also have a ESPHome template available which can be easily flashed via [this website](https://planet-laterna.github.io/Laterna-ESPHome-template)

<h5>Required steps for manual flashing</h5>

* First you need to put the Board in flash mode
* Option 1: Press and hold the Flash button before connecting the board to USB or programmer connector. Rlease the flash button after you connected the board.
* Option 2: Press the Reset and Flash button while the board is connected. The release the Reset button first and then the Flash button.


<h3>PINOUT Description</h3>

<img src="/Pinout/Pinout.png" width="50%">

<h3>Circuit protection</h3>

this board includes 1 resetable fuse to limit current on the board.
<br>If powered by external power supply -> 3A

We recommend to power the module by using a USB power supply or external powersupply. **DO NOT POWER LED Strips directly from laptop/PC port**

<h5>Tested 5V LED Strips:</h5>
<br>WS281x</br>
<br>WS2801</br>
<br>SK6812</br>
<br>
Please take note that this Laterna Version **only support 5V LED Strips and Power Supplies**.


<h3>Use Cases - Videos</h3> 

[![Alt text](https://img.youtube.com/vi/_RJb7WULv-4/0.jpg)](https://www.youtube.com/watch?v=_RJb7WULv-4)

**Plug and play example - Simple Connection**

[![Alt text](https://img.youtube.com/vi/4foqMvrpt0A/0.jpg)](https://youtu.be/4foqMvrpt0A)


* plug and play example - External power supply
* Adding a button
* Adding a sound sensor
* Adding a distance sensor
* etc
(**Work in Progress**)

<h3>License</h3>

Software used in this guide is open source and licensed under the **MIT License**

<h3>FAQ</h3>

* Can I use this board with my own code?
  - yes, you can write your own code and programm this board. Refer to programming steps section
* How many LEDs can I control with this board?
  - we recomend to use xx LEDs if board powered by USB and yy LEDs if powered with external power supply (**Work in Progress**)

<h3>Acknowledgment</h3>

We would like to thank WLED Developers for their great job, our platform relies strongly on their work
[![Alt text](https://github.com/Aircoookie/WLED/blob/master/images/wled_logo_akemi.png)](https://github.com/Aircoookie/WLED)
