# NB-RetroGames

**Instructions:**

Insert blank micro SD card into computer.
Download Raspberry PI Imager https://www.raspberrypi.org/software/ 
Install for your device (Windows or Mac).
Open Raspberry Pi Imager and select ‘CHOOSE OS’.
go to ‘Emulation and game OS > Recalbox (Pi4).
Select ‘CHOOSE SD CARD’ and select your SD card from the list.
Select WRITE  (This will take around 15mins.).
Remove SD card and insert.

**Configure Controllers**
On first start up a pop up will say x Gamepads detected, hold a button on your device to configure it.
Hold any button down to go to the mapping screen and assign all the buttons appropriately (FYI- North East South West is Triangle, Circle, X, Square.
Ensure to assign select as the hotkey enable button
To change/add new controllers including wireless controllers go to main menu > Controllers settings

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
