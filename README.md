# WinDeckOS [Version 1.1]
Simplifying Windows on Steam Deck with a custom image that makes it feel much more like steamOS and includes many ease of use additions. 
#
Some of the most noteable changes are:
1. All steam deck drivers come pre-installed
2. It starts with the same UI steamOS uses, so you can keep the console like experience and still get the better compatibility windows brings. Best of both worlds.
3. Sleep mode is fully working here
4. The WiFi driver is greatly improved due to the usage of the [RTKiller driver](https://github.com/ryanrudolfoba/SteamDeckWindowsFixForWiFi)
5. A whole bunch of other quality of life stuff, a full list can be found [here](https://drive.google.com/file/d/1fPM4LSM65I5WNBEaw7nCKSlL4Tl3zcg4/view?usp=drive_link)

# Video Tutorial
[A video showcasing how to install WinDeckOS can be found here:](https://vimeo.com/844086829?share=copy) and if that video is taken down, [then you can find it here](https://drive.google.com/file/d/1rKiU0uRroSsQrylyUChOw32mEfZ6DDlP/view?usp=sharing)
#
And if neither of those work, [this one should](https://mega.nz/file/8uUFUTQK#I_z8_MpOg-dhXvq4wXZBu1bBcVCm4Ga-ZkGZxFnyZTA)

## Links mentioned in the video guide
["Media Creation tool"](https://go.microsoft.com/fwlink/?linkid=2156295)  ["MacriumRescueISO and WinDeckOS download"](https://api.mod.io/v1/games/1673/mods/3157675/files/4032600/download)   
["Rufus"](https://github.com/pbatard/rufus/releases/download/v4.1/rufus-4.1.exe)
### Alternative Download Links
["MacriumRescueISO Alternate link"](https://mega.nz/file/xvkxxKKI#tsEXHTpIX7ZUx9xDvh73mfA_HRsE8CI3XBWzmvGY1ZI)   ["WinDeckOS Alternate Link"](https://mega.nz/file/QqdV1Dob#wWDaDDJnLDR5BjmpLbQS3K2TXA_d2DAw9QI52yAp1bo) 
[MacriumRescueISO Google Drive Link](https://drive.google.com/file/d/1n7WgFMYcTdNSrqaJQW_xnqlQtnmZSM-9/view?usp=sharing)   
[WinDeckOS Google Drive Link](https://drive.google.com/file/d/16ohIRz1HAWFYw96h0gfDETL4LuRRLhrf/view?usp=sharing)
["WinDeckOS Patch Notes"](https://drive.google.com/file/d/1fPM4LSM65I5WNBEaw7nCKSlL4Tl3zcg4/view?usp=drive_link)
#
And [here's an alternative link that should be working for everyone that contains the MacriumRescueISO and the WinDeckOS image file.](https://api.mod.io/v1/games/1673/mods/3157675/files/4032600/download) 
Using mod.io as every other site is filled to the brim with download restrictions.



# Written Guide
This is a written guide explaining how to install WinDeckOS using an external Windows PC.

## Requirements
1. An external PC running Windows
2. Some kind of external storage device with at least 12GB of usuable storage and a way to connect it to your Steam Deck
3. A Steam Deck (or maybe some other device you want to try downloading this too)

It is recommended that the external storage device contains at least 16GB, although technically, as long as there is 12GB of usuable memory, this should work.
This should work on an SD card, although I haven't tested that personally so I can't confirm anything.
This will completely wipe your steam deck, so be sure to back up any files, such as saves, you wish too keep. Not every steam game supports cloud saves so keep that in mind before continuing.

# Step One: Formatting the Deck's Drive
You can skip to step 2 if you already have windows installed, or if the drive your using is already completely wiped
#
### Media Creation Tool
Download the Media Creation tool for windows [here.](https://go.microsoft.com/fwlink/?linkid=2156295) Once it's finished downloading, run it, and make sure your external storage device is connected. 
Accept the windows license agreement and when asked about language and edition, choose whatever you want and click next. When asked which media to use - enseure you click "USB flash drive", then click next. Select the external drive your using for setup, then click next. 
The installer will tell you that your device is ready and you can now safely close it and insert the drive into your Steam Deck.
### Booting the external drive
Ensure your external drive is connected to your Steam Deck and then hold down the volume down key and press the power button one time. Your deck will beep and then it should boot into the Bios. From here, select whatever external drive your using for setup and it should
boot the windows installer in vertical mode.
### Formatting the drive from the windows installer
The trackpad is still controlled as if the screen was horizontal so navigation can be a bit tricky, but the touch screen does work if you'd prefer to use that. On the first screen that shows up, click on next and then install now. When asked about a product key, select 
"I don't have a product key". It doesn't matter what version of windows you select, so just click next (Your version of windows will be the same regardless of your choice here). Accept the license agreement and then select next.
# 
(If you have an SD card inserted that you don't want too wipe, then you should remove it before doing this part, unless you used an SD card to create windows installation media)
#
When asked whether to "Upgrade Install" or "Custom Install" ensure you select "Custom install". You will then be greeted with a screen full of drives and partitions. Manually go through and select each drive then click delete, then format the remaining ones it lets you. 
After doing this, your steam deck will no longer boot. Once your done, you may hold down the power button on your steam deck to shut it off.
# Step Two: Preparing the drive for installation on the Deck
Make sure your external drive is connected, and start downloading the [MacriumRescue ISO and the WinDeckOS disk image](https://api.mod.io/v1/games/1673/mods/3157675/files/4032600/download)
#
While those are downloading, download this program called [Rufus,](https://github.com/pbatard/rufus/releases/download/v4.1/rufus-4.1.exe) and run it. On the auto update box, you can select "no". In the rufus UI, select the external drive your using. 
If your drive isn't showing up, you may need to select "Show advanced hard drive properties" and check the box titled "list USB Hard Drives". Under the "Boot selection" tab, there's a select button that will let you browse for a file, 
in this case select the [MacriumRescue ISO](https://api.mod.io/v1/games/1673/mods/3157675/files/4032600/download) we downloaded earlier, or just drag and drop the file into Rufus. Make sure the "Partition scheme" is set too GPT 
and the "File system" is set too "NTFS". Everything else should remain unchanged. Press "Start" and you will get a popup warning you that the drive will be formated. Press "ok" and wait for it too complete.
#
Once it finishes, open the newley changed drive in file explorer (should be labled "Rescue"), and drag and drop the [WinDeckOS image file](https://api.mod.io/v1/games/1673/mods/3157675/files/4032600/download) to the root of the external drive 
(This may take awhile). Once it finishes, take out the drive and put it in your Steam Deck.
# Step Three: Installing the image onto the Deck
Ensure your external drive is connected to your Steam Deck then hold the volume down key and press the power button one time. Your Steam Deck should beep and boot into the Bios. from here select the external drive your using for this setup and it will boot the Macrium 
Reflect ISO in vertical mode. Select "Browse for an image file..."
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/459a3c6a-5a8e-4956-abdd-01acba91e28e)
#
In the "Select an image file" window choose the drive labeled "Rescue"
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/654af02d-5a8d-463b-a0da-48c6988135db)
#
Choose the file named WinDeckOS
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/dac48fc1-6a2a-46aa-8294-882d5644d47a)
#
Click the first of the three new boxes on screen and a button called "Actions.." will appear
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/98225ce8-419f-4cc2-958c-33c30f87dd78)
#
Afther clicking "Actions..." you'll need too select "Restore this partition..."
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/ae08f404-c3a4-4d2a-a9d9-d13058fbfe69)
#
Click on "Select a disk to restore to..." and you'll be met with a bunch of options.
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/7ee58c03-4d47-476c-b1f1-e3654df7abb7)
#
Choose the drive you wish to install WinDeckOS too (it's recommended you install it to the internall SSD or things like sleep mode may not work). Next, check all 3 of the little boxes from the disk image (you may need to drag the window too make the last box visible)
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/617e321b-43a2-4310-b444-fc67cf1445c3)
#
Once they're all checked, click "Copy Partitions" then select "Shrink or extend to fill the target disk". If you don't get that prompt, don't worry, it's because you have a 2TB drive and the partitions already fit that.
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/6edfd3ad-ceab-435a-84a9-165c6bacb29c)
#
If done correctly, every box will have a green outline around it, like this;
#
![image](https://github.com/Minibattle/WinDeckOS/assets/67839290/d3fe805b-6fd6-4c81-b3ad-0dd5afa6d902)
#
Click "Next" in the bottom right and then click finish (may require you too drag the window for that option to be visible). You'll get a prompt stating that the drive will be formated, check the acknowledgement box then press continue. 
From here, WinDeckOS will start installing and once it's finished you can restart your Steam Deck and it should boot into WinDeckOS.
# Step Four: First Time Setup
WinDeckOS may boot in vertical mode, if this is the case, wait for the gamepadUI too show up and once it does swipe 3 fingers down to be taken to the desktop. Click the windows button on the taskbar and head to settings. Then click on display, scroll down too display
orientation, and change it too "Landscape". Close settings and tap the steam icon on the taskbar to open the gamepadUI again proceed with setup, and when you get too Wifi there's two ways to connect.
### Option One: Connecting manually by typing in the network SSID
In the gamepadUI select "Other network..." and type in your internet information. Next, select your WiFi at the top of the list and finally, sign into your steam account and you'll be done with the WinDeckOS setup and ready to go.
### Option Two: Connecting from the desktop
Swipe 3 fingers down to show the desktop, and in the bottom right tap the internet icon located next to the sound and batter icon. In the quick access menu that shows up, tap the arrow next to the WiFi symbol and connect to your internet using the touch screen. After doing so, tap the steam icon and you will need to restart your steam deck, or you won't be able to type on the sign in screen. Simply press the steam button, go down to power, then press "Restart System". 
After that proceed through the setup as normal and you will be fully setup with WinDeckOS. Enjoy!


