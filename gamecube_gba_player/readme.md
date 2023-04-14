# gamecube_gba_player

## GBA Player Overview
Shows how to use Nintendo Gamecube with Gameboy Player and freeware software to play gameboy/color/advance games on HD television, with an SNES controller.

## Parts required
Gamecube
HDMI converter, or Gamecube component cables (very expensive)
SNES controller adaptor
Zelda Wind Waker gamecube disk
SD card (full size, regular speed. 2GB)
SD to Gamecube memory card adaptor
Standard gamecube memory card (144 blocks)

## Copy gamesave to game card (on Wii)
Main steps I followed are here:
2 GB Full Size SD card, Fat16 format, files include:
	autoexec.dol
	apps/gcmm/boot.dol
Need to use my Wii which is softmodded and previously had Wii Homebrew channel installed
Open Homebrew channel on Wii, see bubble screen. Insert SD card (or SD card in Gamecube converter) and blank GC Memcard
Select the GCMM (gamecube memory manager) application. Format the memory card. Then restore gzle.gci (windwaker save hack) and restore GCMM or swiss?
Now that you have your memory card with windwaker save hack, and GCMM/swiss, put it in your gamecube.
Load gamecube with windwaker disk. Press start. The system will freeze. Should launch the GCMM/swiss app.
Using Swiss, you can launch the gci.dol to load gameboy interface. Options menu is seen first for 240p, etc.


## Tutorial

### Intro
To run GBI, you need to run the homebrew app from a gamecube memory card.
I used the Zelda Wind Waker save file hack to launch the homebrew app (swiss or gbi).
Use gcmm app from a Wii with HomeBrew channel to copy windwaker save and swiss to GC memory card from SD card. (gci files in MCBACKUP)
In gcmm, "restore" is copy gci file from SD card to gc memory card. "backup" is copy memorycard save to SD card in .gci format
The homebrew channel on Wii shows blank bubble screen by default. Plugin SD card with apps folder and it automatically shows the apps.

### Overview
	Run the GBI (Gameboy Interface) custom software with Gameboy player on Gamecube
### Setup
	Use wind waker save hack to launch the homebrew from a memory card
	Setup gamecube with gbplayer, gba game, snes to gc controller, windwaker disk, memorycard with ww save hack and gbi/swiss apps.
	Power on gamecube, hit start on windwaker title screen. system freezes, then launches "boot.dol" from memory card (gci format)
### Create SD card
	Copy software to SD card (low speed, 2GB or less, FAT16 format. Do not delete any files from SD - reformat. Needs contiguous memory)
	Root of SD has 
	MCBACKUP on SD has boot.gci, gzle.gci (windwaker US hack savestate)
### Create memory card
	Plug SD card to Wii, launch homebrew channel, launch gcmm. Format memory card in my region. Copy gzle.gci save. Copy swiss.gci



## How to boot the GBI Interface
To play a GBA game, insert when console off. Power on and follow these steps:


## Definitions:
	swiss: app to launch other homebrew apps. Homebrew hub
	gcmm: gamecube memory manager. format and copy to and from gamecube memory cards
	GCMM is 3rd party memory card manager
    dol: file format for dolphin/gamecube applications
	gci: file format for gamecube save files
    .gci == hacked game save and homebrew loader files
	gzle.gci: USA/Everywhere region of windwaker hack save
	bootmii: low level app, insurance in case your wii bricks. backup the wii NAND flash
	hackmii: 
	GBI: gameboy interface. homebrew alternate software for gameboy player disk
    Swiss: lets you run homebrew apps

## Links
- Great: https://www.gc-forever.com/forums/viewtopic.php?f=39&t=3311
- Wind Waker exploit save: what it does it load a boot.dol from your memory card.
- https://github.com/FIX94/ww-hack-gc/releases/download/v1.1.1/WWHack-GC-v1.1.1.zip
- GCMM: http://wiibrew.org/wiki/GameCube_Memory_Manager
- https://www.youtube.com/watch?v=_znAYi585QE
- Gamecube GBI gameboy interface: https://gchomebrew.com/ultimate/
- How to transfer Gamecube save files with SD card: https://www.youtube.com/watch?v=mihAzBQieqo
- MetalJesus talks Gamecube mods: https://www.youtube.com/watch?v=PpTSDUYCq1o

- https://www.youtube.com/watch?v=vITs5bTP7QQ (Everything Homebrew in 6 minutes)
Says you need FAT32 SD card
Region printed on the disk
GXXJ (Japan)
GXXP (PAL)
GXXE (Everywhere else)
Need to use GCMM on WII to create the hacked memory card backup
## GCMM can only backup game saves in MCBACKUP folder on SD card
Carby V2 HDMI - best and cheapest HDMI adaptor ($80)
Wind waker: gzlp.gci (PAL) gzlj.gci (japan) gzle.gci (Everywhere)
ROOT\gcmm_14f.dol
ROOT\MCBACKUP\boot.gci
ROOT\MCBACKUP\gbi-20200609.gci
ROOT\MCBACKUP\gzle.gci

- https://www.gc-forever.com/wiki/index.php?title=Game_Boy_Interface (Game Boy Interface Wiki)
Carby v2 HDMI Adapter
.gci == hacked game save and homebrew loader filesSD card with Swiss and a hacked game save
Wind waker hack: insert disk, insert the gamecube memory card (with hacked save), hit start button on title screen
hacked game save will cause game to glitch, then load swiss. then you can load anything
2m 13s - show how to use GCMM
Action reply - slow. only useful to load swiss.dol from SD card, to then load GCMM.dol, to create hacked game save
need 251 block game save card (16mbit) (2mbyte)
Software only works with 2GB or less slow full size SD card
SD Gecko: lets you put SD card into memory card slot
Memory card slot A and B are SPI (Serial Peripheral Interface) boards. Some software can't read SD card, only memory card (EXI)
SD2SP2: plug
DOL-001 (serial port 2 on bottom, digital video out)
Cannot delete files on SD card - need to format and copy over again)



## Random notes

-------
Gamecube

Get the GBI to load Metroid Fusion on gamecube gbplayer on large CRT TV with S-Video.
GCMM is 3rd party memory card manager
Download gci file (game save) to MCBACKUP
Boot up GCMM.dol
Restore the GCI file (copy to memory card)
Wii transfer
MS.GCI

-----------------
Wii

My wii has homebrew channel app. Hit home button to launch bootmii
If 512mb SD card is plugged into Wii, I can launch BootMII from SD card. Use wii power/reset buttons for menu
HackMii v0.8 installer
Install BootMii as insurance in case your wii bricks




