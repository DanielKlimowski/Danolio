# How to install Bongo Cat mod on the Satisfaction75 r2 

![bongocat](https://upload.wikimedia.org/wikipedia/commons/9/97/Bongo_Cat_Redraw.png#center)

## Getting started
The purpose of this guide is to install and enable the BongoCat animations for firmware on embedded OLED screens, such as Cannon Keys’ Satisfaction75 R2 keyboard. 

### You will need:
* A built Satisfaction75 r2 keyboard and usbc cable (I am not sure if this will work for the first release version Satisfaction75 R1)
* [QMK Configurator](https://docs.qmk.fm/#/)
* [A copy of the Satasfaction75 firmware which includes the BongoCat mod](https://github.com/pedker/OLED-BongoCat-Revision/blob/main/cannonkeys_satisfaction75_rev1_Pedker.bin) 
* A computer which can store and open files locally

## Step 1: Download the newest release of QMK Configurator
To install QMK Configurator on your PC: download the installer from QMK's GitHub: https://github.com/qmk/qmk_toolbox/releases

Download the file labled "qmk_toolbox_install.exe" circled in red below 
![image](https://danielklimowski.github.io/bongocatassets/1.png)

Once the file has finished downloading: click on it to run the file
![downloaded file](https://danielklimowski.github.io/bongocatassets/2.png)

Upon running the file you will be presented with this prompt. Select "Yes" ![prompt1](https://danielklimowski.github.io/bongocatassets/3.jpg)

You will then be able to choose where to save the program. The default location will be fine, so select "Next"
![save](https://danielklimowski.github.io/bongocatassets/4.png)

Next, select "Install" to install QMK Configurator ![install](https://danielklimowski.github.io/bongocatassets/5.jpg)
Once QMK Configurator has finished installing, close the application and proceed to the next step. 

## Step 2: Download the Satasfaction75 BongoCat firmware

To display the BongoCat mod on the Satasfaction75's OLED you will need to flash the keyboard with a copy of the firmware which contains the mod

The modded firmware can be downloaded [here](https://github.com/pedker/OLED-BongoCat-Revision/blob/main/cannonkeys_satisfaction75_rev1_Pedker.bin). Click the download widjet to save a copy of the firmware. Remember where you save this file as you will need it later. 
![something](https://danielklimowski.github.io/bongocatassets/6.jpg) 

## Step 3: Flashing the keyboard
Ensure that your keyboard is unplugged ![unplugged](https://danielklimowski.github.io/bongocatassets/7.jpg)

If your keyboard is assembled, you will need to remove the backplate to gain access to the PCB. There are eight (8) screws which must be unscrewed to remove the backplate![screwlocations](https://danielklimowski.github.io/bongocatassets/8.png)

Once you have access to the PCB, ensure the boot switch is in position "1" ![pcbunpluggedpos1](https://danielklimowski.github.io/bongocatassets/9.png)

Plug in the keyboard ![exposedpcbpluggedin](https://danielklimowski.github.io/bongocatassets/10.jpg)

Open QMK toolbox. 

In the rightmost dropdown menu ensure that "ATmega32U4" is selected. Then click on the open button to select a firmware file ![openfile](https://danielklimowski.github.io/bongocatassets/11.jpg)

Select the.bin file which contains BongoCat mod then select "Open" ![bongocatfile](https://danielklimowski.github.io/bongocatassets/12.jpg) 

Once you've selected "cannonkeys_satisfaction75_rev1_Pedker.bin" click the "flash" button ![clickflash](https://danielklimowski.github.io/bongocatassets/13.png)

After flashing QMK will display the message "Flash complete" ![flashingdone](https://danielklimowski.github.io/bongocatassets/14.png)

Return the switch on the PCB back to the 0 position ![switchtozero](https://danielklimowski.github.io/bongocatassets/15.png)

Press the reset button ![pressbutton](https://danielklimowski.github.io/bongocatassets/16.png)

Now that the keyboard is flashed: reassemble the keyboard

## Step 3: Using VIA to enable BongoCat on OLED display
With the keyboard flashed, we just need to enable the BongoCat mod using a configurator. We can do this using [VIA](https://usevia.app/)

Go to VIA's website: https://usevia.app/ and click the "Authorize device" button at the bottom of the screen ![click](https://danielklimowski.github.io/bongocatassets/17.png)

In the window that pops up select Satasfaction75, then click "connect" ![connectdevice](https://danielklimowski.github.io/bongocatassets/18.png)

After allowing VIA to connect to the keyboard we can use it to alter the OLED display settings. Click on the "CUSTOM FEATURES" widget in the bottom left of the HUD. ![OLEDsettings](https://danielklimowski.github.io/bongocatassets/19.png) 



In custom features you can configure the settings of the Satasfaction75's OLED screen. "Default OLED Mode" determines which mode will be displayed when the keyboard is turned on. Current OLED Mode determines which mode is currently displayed. There are three modes to choose from:

| OLED Mode | Display | Description
| ------------- |:-------------:| :---------: | 
| Default | ![default](https://danielklimowski.github.io/bongocatassets/20.png) | Displays BongoCat, clock and WPM (words per minute) tracker
| Time | ![time](https://cdn.discordapp.com/attachments/552500104678998016/1123737748164071464/image.png) | Displays a solitary centered BongoCat
| Off | ![off](https://cdn.discordapp.com/attachments/552500104678998016/1123737805357592637/image.png) |Displays default Satasfaction75 OLED hud

Changes to the settings will be applied automatically. Once you've changes settings as desired, feel free to close the browser.  

## Tah-dah!
You've now enabled BongoCat on your Satasfaction75! Enjoy! :3

![image](https://danielklimowski.github.io/bongocatassets/21.gif)


