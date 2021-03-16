# NC-RetroGames Systems

**Set-up Instructions- Please note that due to copyright laws I cannot provide the game playing software or the games themselves. However it is easy to do and i'm happy to help out if you encounter any issues!** NB: Video guides can be found in the How to Guides section

**Install recalbox Operating system**
Insert blank micro SD card into computer (Open the disc drive
Download Raspberry PI Imager https://www.raspberrypi.org/software/ 
Install for your device (Windows or Mac).
Open Raspberry Pi Imager and select ‘CHOOSE OS’.
go to ‘Emulation and game OS > Recalbox (Pi4).
Select ‘CHOOSE SD CARD’ and select your SD card from the list.
Select WRITE  (This will take around 15mins.).
Remove SD card and insert back into console (microchip side down)

**Configure Controllers** NB The front ports are designed to accept original PS1 controllers. USB controllers can be plugged into the rear usb along with Bluetooth controllers
On first start up a pop up will say x Gamepads detected, hold a button on your device to configure it.
Hold any button down to go to the mapping screen and assign all the buttons appropriately (FYI- North East South West is Triangle, Circle, X, Square.
Ensure to assign select as the hotkey enable button
To change/add new controllers including wireless controllers and change the assigned player 1/2/3/4 controllers go to main menu > Controllers settings

**Enable Power/RESET Buttons and Power LED**
Follow this video guide...
or
In Web browser type \\RECALBOX
Username is root
Password is recalboxroot
On left hand menu select recalbox.conf
In the text file delete the semi colon ; before the following lines near the top
;system.power.switch=PIN56PUSH           # https://github.com/recalbox/recalbox-os/wiki/Add-a-start-stop-button-to-your-recalbox-(EN)
;system.power.switch=PIN356ONOFFRESET    # https://github.com/recalbox/recalbox-os/wiki/Add-a-start-stop-button-to-your-recalbox-(EN)

Click save. Then restart console using the controller. Buttons will now be working

Please Note You must wait for the system to fully power down before unplugging as doing so will corrupt the SD Card
Also please wait a few seconds after shutting down before attemping to turn on again. 
System can take 30 seocnds to boot and will show blackscreen and the LED will turn off briefly. Please be patient :)


**Set Audio Output to HDMI/3.5mm Headphone Jack**
Go to Main Menu > Sound Settings > Output Device   (NB- Set front end Music to Off to remove the preset music from the menu)

**Reconfigure Theme/Skin**
Go to Main Menu > UI Settings > Theme Set- RECALBOX-NEXT   (NB You can pick any other theme you like
Next go to Theme COnfig > Theme Icons- 5-PSX to enable PS1 button icons

**Enable Wi-FI**
Press Start > Network Settings > Enable WiFi- ON
Goto to WiFi SSID and enter your network name
Go to WiFi Key and enter your Password

**Transfer Games/BIOS** **NB** **It is essential that you upload a BIOS file onto the system as this will help run the games much smoother. A video guide can be found here ****

Follow the video guide here..
or
In file explorer address bar type   \\RECALBOX
Username is root
Password is recalboxroot
Open Share > Roms > PSX and just drag and drop files in **NB Make sure all files for each game are added including the .cue .sub .ccd .bin .img files as games will not work otherwise**
Go back to share , then > BIOS and add all of the BIOS files from the PS! BIOS files link above (should be 6 scphXXXX.bin files, XXXX are numbers)

**Link for Playstation 1 Games** https://the-eye.eu/public/rom/Playstation/Games/NTSC/  **Note I do not sell consoles with games or provide my own game content as this would be copyright infringement. 

**After unzipping these files I recommend renaming those that do not match their official name eg: Change GTA2 to Grand Theft Auto 2 to help the system find the artwork etc

**Add Original PS1 startup/other custom startup** NB There is a copy of the original PS! start up video in the How to Videos Section
In file explorer type in \\RECALBOX
go to system > resources > splash
delete all other files in the folder and copy your desired video into the folder
Put the intro video file in recalbox/system/resources/splash and delete all other video files
