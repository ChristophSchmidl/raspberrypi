# Raspberry Pi

Things you need in order to have a working Raspberry Pi setup:

* Raspberry Pi Board
* Power Supply
	* Any micro USB power supply around 2500 mAh should be enough. Note: Try to avoid power supplies with 1000 mAh because that won't be enough to sufficiently supply your Raspberry Pi and its peripherals.
* SD Card
	* You can choose whatever you like but the card should be large and fast enough. The Samsung Evo Select 32GB is a good choice and does not cost much.
* Screen
	* If you use your TV with the Raspberry Pi then you need a normal **HDMI cable**. If you want to use your TV's remote control with the Raspberry Pi then your TV should support the **HDMI Consumer Electronics Control (HDMI-CEC)**, otherwise you have to buy another remote and an adapter for your Raspberry Pi (e.g. FLIRC USB (2nd Gen) Universal Remote Control Receiver For Media Centre).
	* If you do not use your TV then you probably want to have something similar to a TFT LCD Touchscreen Monitor designed for the Raspberry Pi 
* Input devices
	* Keyboard and Mouse. There are also plenty of combo devices which also include a wireless adapter for your Raspberry Pi (e.g. Logitech K400 Plus Keyboard).
* Case (optional but nice to have)




## Raspberry Pi

Note: If you want to buy a new Raspberry Pi in 2018/2019 then you should go with the **Raspberry Pi 3 Model B+** because it is approximately 20% faster than the Raspberry Pi 3 model B and only costs slightly more.


The following list contains all Raspberry Pi versions in historical, descending order:


* Raspberry Pi 3 Model B+: Announced on "Pi Day", 14th March 2018
	* German Amazon: 38,50€ (https://www.amazon.de/Raspberry-1373331-Pi-Modell-Mainboard/dp/B07BDR5PDW/ref=sr_1_5?s=computers&ie=UTF8&qid=1544188843&sr=1-5&keywords=raspberry+pi+3+b%2B)
	* American Amazon: 38.88$ (https://www.amazon.com/ELEMENT-Element14-Raspberry-Pi-Motherboard/dp/B07BDR5PDW/ref=sr_1_3?s=pc&ie=UTF8&qid=1544188889&sr=1-3&keywords=raspberry+pi+3+b%2B) 
* Raspberry Pi 3 Model B: Announced on 29th Feb 2016
	* German Amazon: 31,49€ (https://www.amazon.de/Raspberry-Pi-Model-ARM-Cortex-A53-Bluetooth/dp/B01CD5VC92/ref=sr_1_5?s=computers&ie=UTF8&qid=1544188979&sr=1-5&keywords=raspberry+pi+3+b)
	* American Amazon: 36.70$ (https://www.amazon.com/Raspberry-Pi-RASPBERRYPI3-MODB-1GB-Model-Motherboard/dp/B01CD5VC92/ref=sr_1_6?s=electronics&ie=UTF8&qid=1544188922&sr=1-6&keywords=raspberry+pi+3+b)
* Raspberry Pi 2 Model B: Announced on 2nd Feb 2015
* Raspberry Pi Model B+: Announced on 14th July 2014 

For a full description, see: https://elinux.org/RPi_HardwareHistory


## SD Card

* https://www.amazon.de/Samsung-microSDHC-MB-ME32GA-EU-Speicherkarte/dp/B07CXXBTST/ref=sr_1_1?ie=UTF8&qid=1544190328&sr=8-1&keywords=samsung+evo+select+32gb


### Flashing the SD card on Mac OS (propably the same on Linux)

Tutorial: https://computers.tutsplus.com/articles/how-to-flash-an-sd-card-for-raspberry-pi--mac-53600

Download an image for the Raspberry Pi like LibreElec (https://libreelec.tv/downloads/) and uncompress it into an .img file. Put the sd card into your mac, open up the terminal and type:

```diskutil list```

This will show all disks on your machine. Look for your sd card by inspecting the different sizes of your disks. Your sd card is probably listed under **/dev/disk3**.


```diskutil unmountdisk /dev/disk3```

This will unmount the disk so you can actually work with it. Navigate to the location where you stored your image and type:

```sudo dd if=LibreELEC-RPi2.arm-8.2.5.img of=/dev/disk3 bs=2m```

Wait a bit for the program to finish and you are done. Put the sd card into your Raspberry Pi and let the OS start.


## Power Supply

* https://www.amazon.de/T%C3%9CV-HKY-Ladekabel-Ladeger%C3%A4t-Smartphones/dp/B06XKYSQSD/ref=sr_1_19?ie=UTF8&qid=1544190245&sr=8-19&keywords=micro+usb+netzteil
* https://www.amazon.de/HomeSpot-Raspberry-Ladeger%C3%A4t-Netzschalter-Kompatibel/dp/B078567K85/ref=sr_1_6?ie=UTF8&qid=1544189942&sr=8-6&keywords=micro+usb+netzteil


## Case

* https://www.amazon.de/anidees-AI-PI-SG-Plus-Raspberry-Aluminium-Acryl-Top-Deckel/dp/B00SV8HTAC/ref=pd_sbs_147_6?_encoding=UTF8&pd_rd_i=B00SV8HTAC&pd_rd_r=cb86ae74-fa27-11e8-ae0b-17997801fa7c&pd_rd_w=G26Ou&pd_rd_wg=ZoQG2&pf_rd_p=51bcaa00-4765-4e8f-a690-5db3c9ed1b31&pf_rd_r=HMB2N3NVY70CX6J04P3T&psc=1&refRID=HMB2N3NVY70CX6J04P3T
* https://www.amazon.de/FLIRC-Himbeer-Fall-Neues-Modell/dp/B07349HT26/ref=sr_1_3?ie=UTF8&qid=1544190358&sr=8-3&keywords=flirc+raspberry+pi+3
* https://www.amazon.de/NES-Geh%C3%A4use-Raspberry-Model-Kintaro/dp/B01M4OOY4U/ref=sr_1_2?ie=UTF8&qid=1544190423&sr=8-2&keywords=snes+case+raspberry+pi+3
* https://www.amazon.de/YIKESHU-Retroflage-Funktionale-Reset-Taste-Controller/dp/B07HH7W8GW/ref=sr_1_4?ie=UTF8&qid=1544190423&sr=8-4&keywords=snes+case+raspberry+pi+3

## Raspberry Pi for Audio

* https://www.balena.io/blog/turn-your-old-speakers-or-hi-fi-into-bluetooth-receivers-using-only-a-raspberry-pi/#hardwarerequired
* http://www.hifi-forum.de/viewthread-181-11004.html
* https://www.max2play.com/2019/11/raspberry-pi-hi-fi-streamer-mit-7-zoll-touch-display-und-hifiberry-soundkarte/
* https://www.hifiberry.com/

