# Snes9x RX
https://github.com/niuus/snes9xrx/

Based/forked from:
https://github.com/snes9xgit/

https://github.com/dborth/snes9xgx/

(Under GPL License)

Snes9x RX is a Super Nintendo™ / Super Famicom emulator for the Nintendo Wii.
Snes9x RX is a fork from Snes9x GX, a port of Snes9x (http://www.snes9x.com).

Snes9x RX is a "homebrew application" which means you will need a way to run
unsigned code on your Nintendo Wii. The best website for getting started with
Wii homebrew is WiiBrew (www.wiibrew.org).


## FEATURES

* Core based on Snes9x 1.52 for max performance.
* MSU-1 co-processor support, for full-motion video & CD-quality audio!
* Satellaview boot support through the use of the add-on's original BIOS.
* Wiimote, Nunchuk, Wii Classic/Classic Pro, and Gamecube controller support
* Wii U Pro, Wii U GamePad, NES and SNES Classic controller support
* Retrode 2 USB adapter support, so you can use the real controllers!
* Mayflash PC044 and MF105 SNES to USB adapter support
* Wired Xbox 360 Controller support (autodetected when in-game)
* Speedlink Hornet Gamepad USB
* Experimental DualShock 3 support
* SNES Superscope, Justifier, Mouse peripherals emulation support
* Cheat support
* Auto Load/Save Game Snapshots and SRAM
* Custom controller configurations
* SD, USB, DVD, SMB, Zip, and 7z support
* UStealth USB devices support
* Autodetect PAL/NTSC, 16:9 widescreen support
* Video modes: Original (240p) / Filtered (Sharp & Soft) / Unfiltered
* Video filtering modes: None, Scale2x, HQ2x, Scanlines 25%/50%
* Audio filtering modes: None, Sinc, Cubic, Linear, Gaussian
* Remappable Turbo Mode feature - up to 2x the normal speed
* Enable or disable the Sprite per-scanline original console limit!
* Overclock the SNES CPU & Super FX chip at will, to smooth gameplay!
* Zoom option to zoom in/out
* Available in various skins/colors
* Open Source!


## RECENT CHANGELOG

[5.5.0 - December 25, 2022]
* Add B/1 cancel trigger to WindowPrompts. [InfiniteBlueGX]

* Fix initial game selection menu "jump" when using Wii Classic Controller
or Wii U Pro Classic Controller. [InfiniteBlueGX]

* Fix a crash when selecting Cancel after removing a SD/USB device and 
re-opening the app. [InfiniteBlueGX]

* Add B/1 button press to cancel button remapping. [InfiniteBlueGX]

* Remove an unused variable since screenshot button
was moved. [InfiniteBlueGX]

* Upgraded the Cheat engine to newer version. [InfiniteBlueGX]
Previous one still works.

* Languages update: korean, spanish.

[older update history at the bottom]


## INSTALLATION AND USE

On the Wii / Wii U's Virtual Wii, to use Snes9x RX you will need to copy
over the "apps" and "snes9xgx" folders (directories) from the .zip to your
SD Card. It comes pre-packaged in the Homebrew Channel format (which you
will use to launch the emulator). Once you've copied the directories to
your SD Card you will need to place your ROM image(s) into "\snes9xgx\roms"
directory. Optionally, you can place cheat code files and artwork/covers
in their respectively named folders inside the "\snes9xgx\" directory.
If they are not present, the folders will be created at second run, in case
you want to acquire the files later. Once you are done, you can proceed to
run the emulator. Additionally, you can install the Snes9x RX Forwarder
Channel in your Wii or vWii System Menu (it points to "\apps\Snes9xRX"),
or the special Snes9x RX Channel for Wii U, which fully installs to your
console and reads the configuration and necessary files from your device
"\snes9xgx" folder, be it SD or USB.

In the case of the Wii U Channel version, it has the added benefit of taking
advantage of the extra CPU power available, on the condition that you run
the Wii U homebrew app "sign_c2w_patcher" first, to unlock the so-called
"Wii U Overclocked Mode", which simply makes the console avoid the CPU
underclock (729 MHz) to run Wii software at the native Wii U's speed
(1.24 GHz), so it is completely safe to use.

You can use WUP Installer GX2 or the WUP Installer Y Mod to install the
channel, loaded through the Wii U's Homebrew Launcher or through a
WUHB package (Aroma).

After installing the Wii U channel (forwarder) onto your console, proceed
to use whatever special build suits your preference, by unzipping
it to the root of your SD card or USB drive (both on FAT16 or FAT32),
where it will extract the folder "apps" and "snes9xgx", pre-packaged
in their respective .zip archive.

It is important to note, when you use the Wii U's overclocked mode, you
are limited to use the SD as the storage medium for all your files.
No workarounds, as this is currently a console limitation.


## INITIAL SETUP

The first time you run Snes9x RX it will create a new "settingsRX.xml" file
on the SD/USB Card which stores the configuration of the emulator. So when
you run Snes9x RX, it will automatically detect your storage medium and
bring you to the ROM selection screen. If you want to run a game with the
default settings, then just highlight the game and press 'A' on it and it
will load. However, you can configure Snes9x RX to your liking.


## CONFIGURATION

To configure Snes9x RX, press 'A' on the "Settings" box. This will bring
up the "Settings" screen where you can configure the "Saving & Loading",
"Menu", and "Network". You can also restore the settings to their initial 
values by clicking on the "Reset Settings", read the Credits / activate
supported USB controllers (better explained in the USB Controllers section
below), or you can just return to the ROM selection screen by clicking
on "Go Back".


## SETTINGS

### SAVING & LOADING

From this setup option you can configure the way Snes9x RX loads and saves.
Your options are Load Device, Save Device, Load Folder, Save Folder, Auto
Load and Auto Save. Clicking on all of the options will let you toggle
through their settings. Those labeled with "folder" will bring up a text
box where you can enter any other path you wish to use, in case you have
the need to customize it. This is also true for the Cheats, Screenshots,
Covers, and Artwork options.

Snes9x RX has two types of saves - one is the SRAM, which is the save game
data (this is only applicable if the game you're playing supports
battery saving), and the other is Snapshots, which are real time saves.
Real time saves allow you to save your game in it's current state and resume
it at a later time.

```
	• Load Device -	SD, USB, DVD, Network and Auto Detect

	• Save Device - SD, USB, Network and Auto Detect

	• Auto Load - SRAM, Snapshot and Off

	• Auto Save - SRAM, Snapshot, Both and Off
```

You can also toggle the option to append 'Auto' into the filename of all the
automatic SRAM saves that the emulator creates, whenever you play a
supported battery saving cartridge.

### MENU

This settings screen will allow you to customize a few aspects on how the 
Menu works including the Exit Action, Wiimote Orientation (for navigating
through the menus), Music Volume, Sound Effects Volume, Satellaview BIOS
(better explained in the Satellaview section below), Language (all menus),
the type of Preview Image you would like to see on the Choose Game screen,
a toggle to show or hide the "New SRAM" button inside the Save/Load/Delete
menus, and Display Virtual Memory, the latter two shown inside the Game Menu.

The Exit Action can be set to "Return to  Wii Menu", "Power off Wii",
"Return to Loader" or simply "Auto", which will determine the
Exit Action based on the context of how you load the emulator.

### NETWORK

If you're going to be using your Network (LAN) to load and/or save from,
you will need to enter in the SMB share settings you've setup on your
computer via this settings menu. You will need to enter in the SMB Share IP,
SMB Share Name, SMB Share Username and SMB Share Password. If you do not
have a password on your SMB share, then set the SMB Share Password to "0".


## FILE BROWSER (Choose Game)

The File Browser will automatically load when you start the emulator,
listing the contents of the "\snes9xgx\roms\" directory on your SD card
or USB drive. You can specify a different default directory to load games
from (Settings -> Saving & Loading -> Load Folder), or simply navigate to
another one by pressing on "Up One Level", going back as far as the
Device Selection. It will autosave the current directory for you, if you
happen to load any ROM from it. To launch a game (which can be either
uncompressed, or inside a ZIP or 7Z archive) simply click on the title
and it will load. In the case of 7z compressed files, you will be
presented first with a list of all the supported games inside the
compressed archive.


## GAMEPLAY MENU

Once you load a game, you can access a special emulator menu by pressing the
Wii/Wii U controller's 'Home' button / Gamecube controller's 'C-stick Left'.
If you're using any other input controller on the Wiimote extension that
doesn't have a 'Home' button, press 'Start + B + A'. If you use an
special converter to connect other types of controllers on the Gamecube
ports, simply press the button combination 'Start + B + A'. This action
will bring up a special Game Menu that contains the "Save", "Load",
"Delete", "Game Settings", "Screenshot" and "Reset" options.

From this menu, you can also return to the Choose Game screen by selecting
"Main Menu". To leave the menu and resume gameplay, select "Close" or press
'Home' (Wii or Wii U Controllers) or 'Start' (Gamecube controllers).

### SAVE / LOAD / DELETE

The "Save" option will allow you to save either your SRAM (cartridge save
on the internal battery) or a game Snapshot (frozen game state). Once you've
selected "Save", two options will appear named "New Snapshot" - "New SRAM".
Clicking on either of these will create a new save file, which you can
overwrite if you need to by selecting it. The "Load" option will allow you
to load any saved SRAM or Snapshot. Finally, the "Delete" option will let
you select and delete any of your snapshots or SRAM saves.

### SCREENSHOT

This button takes a picture of the screen you're in at the gameplay moment,
for Preview's use on the File Browser's "Choose a game".

### RESET

"Reset" will just reset the game, as the real console behavior.

### GAME SETTINGS

If you pick "Game Settings", you can adjust other special options, which
are thoroughly covered in the following sections.


## GAME SETTINGS

### BUTTON MAPPINGS

Inside the "Button Mappings" settings menu, you can configure the button
mappings for SNES peripherals like the SNES Controller, Mouse, Super Scope,
and the Konami's Justifier. You'll have the option to remap almost all the
controllers already supported by the emulator (except the Retrode 2 USB,
Xbox 360 controller, Hornet Gamepad, or the DualShock 3).

Once you select a controller to configure, you will be presented with a
complete list of the SNES Gamepad buttons you can remap. To set any buttons,
simply pick and click. Snes9x RX will prompt you to press the new physical
button you want to assign to the virtual button you've selected. Below is a
list of each controller, followed by the input devices and the default values
for those devices.

### SNES Controller

		• GameCube Controller

			A = A
			B = B
			X = X
			Y = Y
			L = L
			R = R
			START = START
			SELECT = Z
			UP = UP
			DOWN = DOWN
			LEFT = LEFT
			RIGHT = RIGHT

		• Wiimote

			A = B
			B = 2
			X = 1
			Y = A
			START = PLUS
			SELECT = MINUS
			UP = UP
			DOWN = DOWN
			LEFT = LEFT
			RIGHT = RIGHT

		• Wii Classic Controller
		• Wii Classic Controller Pro
		• Wii U Pro Controller
		• Wii U GamePad

			A = A
			B = B
			X = X
			Y = Y
			L = L
			R = R
			START = PLUS
			SELECT = MINUS
			UP = UP
			DOWN = DOWN
			LEFT = LEFT
			RIGHT = RIGHT

		• Wiimote Nunchuck + Wiimote

			A = A
			B = B
			X = C
			Y = Z
			L = 2
			R = 1
			START = PLUS
			SELECT = MINUS
			UP = UP
			DOWN = DOWN
			LEFT = LEFT
			RIGHT = RIGHT

		• Xbox 360 Controller (wired)

			A = B
			B = A
			X = Y
			Y = X
			L = Left Bumper/Shoulder
			R = Right Bumper/Shoulder
			START = START
			SELECT = BACK
			UP = UP
			DOWN = DOWN
			LEFT = LEFT
			RIGHT = RIGHT
			Left Analog Stick = D-pad directions
			Right Analog Stick = Mapped to Y, X, B, A
			Swap controller port = XBOX GUIDE BUTTON

		• DualShock 3 Controller (wired)

			A = Circle
			B = Cross
			X = Triangle
			Y = Square
			L = Left Bumper/Shoulder
			R = Right Bumper/Shoulder
			START = START
			SELECT = BACK
			UP = UP
			DOWN = DOWN
			LEFT = LEFT
			RIGHT = RIGHT
			Left Analog Stick = D-pad directions

### SNES Mouse

		• GameCube Controller

			LEFT BUTTON = A
			RIGHT BUTTON = B

		• Wiimote

			LEFT BUTTON = A
			RIGHT BUTTON = B

		• Wii Classic Controller
		• Wii Classic Controller Pro
		• Wii U Pro Controller
		• Wii U GamePad

			LEFT BUTTON = B
			RIGHT BUTTON = A

### Super Scope

		• GameCube Controller

			FIRE = A
			AIM OFFSCREEN = B
			CURSOR = Z
			TURBO ON = Y
			TURBO OFF = X
			PAUSE = START

		• Wiimote

			FIRE = B
			AIM OFFSCREEN = A
			CURSOR = MINUS
			TURBO ON = UP
			TURBO OFF = DOWN
			PAUSE = PLUS

		• Wii Classic Controller
		• Wii Classic Controller Pro
		• Wii U Pro Controller
		• Wii U GamePad

			FIRE = B
			AIM OFFSCREEN = A
			CURSOR = MINUS
			TURBO ON = Y
			TURBO OFF = X
			PAUSE = PLUS

### Justifier

		• GameCube Controller

			FIRE = A
			AIM OFFSCREEN = B
			START = START

		• Wiimote

			FIRE = B
			AIM OFFSCREEN = A
			START = PLUS

		• Wii Classic Controller
		• Wii Classic Controller Pro
		• Wii U Pro Controller
		• Wii U GamePad

			FIRE = B
			AIM OFFSCREEN = A
			START = PLUS

### BUTTON MAPPINGS - OTHER MAPPINGS

This sub-menu offers you four options:

```
• Turbo Mode: allows you to turn ON (Default) or OFF the Turbo Mode feature.

• Turbo Mode Button: allows you to remap the feature to any other button, by
cycling through the available labeled options represented on the supported
physical controllers.

• Menu Toggle: allows you to choose which buttons or key combo will be
available to you to return from the game to the Gameplay Menu.

• Map YXBA to Right Stick: offers you the choice to enable the mapping of the
Y+X+B+A buttons to the Right Stick on the supported controllers with analog
joysticks, so shooters like Smash T.V. and Total Carnage are more enjoyable.
If you're using a Gamecube controller, remember to set the "Menu Toggle" to
"Start (PLUS)+B+A" so it doesn't activate fast-forward, or just disable it
by using the "Turbo Mode" toggle.
```

### AUDIO

The Super Nintendo / Super Famicom creates audio through the Nintendo S-SMP,
a wavetable synthesizer and dedicated sound module designed and manufactured
by Sony.

This APU (Audio Processing Unit), which functions as a sound co-processor to
offload the work done by the console's main CPU, mixes up to 8 simultaneous
voices in 16-bit Stereo, at a max sample rate of 32,000 kHz. Sound samples
are stored in the APU's 64KB PSRAM in compressed (BRR) format.

All these samples together are output with a specific process of
audio interpolation, named Gaussian filtering, the APU's native method,
with its own set of pros and cons.

Audio interpolation is a method of making digital audio sound better than
it really is, to improve the listening experience.

The interpolation filter options presented in this menu allow you to fine
tune the produced sound with other filters, which subtly alter the source,
so it's up to your preferences to change it. Below is a short explanation
for each option:

```
• Gaussian: the most accurate representation to how the console sounded.
It minimizes / limits aliasing and might produce better bass in certain
sounds. However, the sound will overall be a bit more muffled or soft,
because of the low-pass filter applied to the sound output.

• Linear: the simplest form of interpolation. Sounds a bit clearer.
The problem with linear interpolation is that it makes straight lines
between each sound sample, and sound waves don't follow straight paths.

• Cubic: might give the brightest sound, it tries to reproduce a more
natural waveform by "bending" the interpolated points around the original
samples. This method gives an interpolating polynomial that is smoother
and has smaller error than some other interpolating polynomials.

• Sinc: Linear and Cubic allow aliasing (this is the misidentification
of a signal frequency, which might introduce distortion or other artifacts
into the recording). Sinc leaves samples sounding essentially as they
do in their raw form.

• None: entirely disables interpolation.
```

The "Stereo Reverse" option will allow you to swap the Left/Right audio
channels, for audio tests, in case your cables are wired different,
or they've been swapped accidentally.

The "Mute" option is self-explanatory. It will completely turn off all
audio output from the game, in case you don't have an inmediate way to
mute your TV or sound equipment. This also has the side-effect of giving you
a couple of extra FPS in-game, due to sound emulation being off the CPU
workload. Pretty much the only games you would notice this speed difference,
are the SNES titles that integrate the Super FX chip.

### VIDEO

The "Video" settings screen will allow you to configure various settings,
including the Rendering method, Aspect Ratio, Filtering, Screen Zoom, Screen	
Position and Video Mode. You can toggle the options for the first three
selections by clicking on them.

```
• Rendering - Unfiltered (Raw pixels)
            - Filtered (Soft)
            - Filtered (Sharp)
            - Original (240p)
            - Filtered

• Aspect Ratio - 4:3 (original)
               - 16:9 correction

• Filtering - None
            - Scale2x
            - hq2x
            - hq2x Soft
            - hq2x Bold
            - Scanlines 25%
	        - Scanlines 50%
```

To use the "Original (240p)" rendering, make sure your LCD/LED display
supports 240p, else you will have a black screen upon returning to the game,
or your display will warn you that there is no signal. This is the most
accurate rendition for the resolution from the original Super Nintendo,
and will give you crisp unfiltered pixels, most ideally suited to enjoy
on CRT TVs / CRT monitors. This rendering mode can even be coupled with
modern TVs for use with scanline generators or line doublers, like the
Framemeister, OSSC, or RetroTink.

Something to keep in mind, the Scanlines 25%/50% filters are not meant
to be used with "Original (240p)" rendering, due to the lower resolution
that's being output. They will make the screen flicker badly.

Also important to note, the Scanlines 25%/50% filtering modes will not
work on games that utilize the Super Nintendo Hi-Res Mode. It will
result in broken graphics (i.e.: A.S.P. Air Strike Patrol) or just no
difference at all (i.e.: Super Buster Bros).

```
• Screen Zoom: this will bring up a menu where you can adjust the Zoom level
by using the clickable left and right arrows. The default setting is 100%.

• Screen Position: this will bring up a screen with four arrows that allows
you to move the position of the video output. You'll only need to use this
option if the screen is not centered. Combining this with the Zoom and
Scaling you should be able to get a proper display on your television.

• Video Mode: manually choose between the supported video standards for
your display. NTSC (480i), Progressive (480p), PAL (50Hz), PAL (60Hz),
or Automatic, the latter one being the recommended setting.

• SNES Hi-Res Mode: this will disable the games capacity to use the
SNES Hi-Res Mode, if you want to use the Scanlines filtering in those
games. It will of course break games that were intended to use the
feature (i.e.: texts in Secret of Mana, Seiken Densetsu 3, etc).

• Crosshair: this will disable the emulator's on-screen crosshair for all
Super Scope / Justifier games.

• Show Framerate: show the frames per second (FPS) on-screen.

• Show Local Time: show the the local time set on your Wii on-screen.
```

### CONTROLLER

Toggle between compatible SNES peripherals that you wish to use your game
with (wherever it is supported), be it two controllers, Multitap (for up to
4 players), Mouse, Superscope, or the Konami's Justifier lightgun.

### CHEATS

This will allow you to enable/disable your Game Genie cheat codes.
Check the in-depth section below.

### EMULATOR HACKS

This will allow you to activate different options that will enhance or alter
the gameplay. Check the in-depth section below.

## CHEATS

Cheats are loaded from the "\snes9xgx\cheats" directory and must be in the
SNES9X .CHT file format. They also must be named the same name as the game
you're playing with the .cht extension. An example would be if you have a 
ROM called "Super Mario World.smc" you would need to name your .cht file to
"Super Mario World.cht". You can find a link to a massive collection of
Super Nintendo cheat codes in the Links section below.


## EMULATOR HACKS

These hacks could significantly alter or improve the gameplay experience,
depending on the game.

```
• Super FX Overclock: this special setting will overclock the speed of
the GSU-1 & GSU-2 chips -most commonly known as the Super FX chip- on every
supported title, which improves games with faster or smoother framerates.
This effect is most notable in games that pushed the original hardware to
its limits, like the Star Fox saga or Doom, for example.

When playing on the Gamecube, whose CPU is slower than the succeeding
consoles, it can give you better speeds on light FX games as
Super Mario World 2: Yoshi's Island.

You can have it at the Default chip speed (10.7 MHz GSU-1 / 21.4 MHz GSU-2),
or set it to 20 MHz, 40 MHz, or 60 MHz. Keep in mind that the majority of
the Super FX games and overclock don't mix well on the Gamecube and it
will slow the games to a crawl, as the console's CPU is not powerful enough.
The same is true with the Wii console, though you can push it to at least
60 MHz without too much trouble, the exception being the game Doom with
anything over 20 MHz, which can leave you with an unresponsive console
depending on the scene.

If you use the Snes9x RX Wii U Channel version along with the console's
"overclocked mode" (by opening the sign_c2w_patcher homebrew before running
the emulator), you can now perfectly enjoy the Super FX Overclock setting
speeds of 80 MHz, 100 MHz, and up to 120 MHz, which give a very nice boost
in framerate for these special games. These last three speed options are
hidden on the Gamecube port, as they are unusable for the reason explained
above.

• SNES CPU Overclock: this special setting will overclock the speed of
the virtual SNES CPU being emulated, which will mostly improve and/or
smooth framerates in games. Drastic examples of improvement are
Out of this World, NCAA Basketball, and the Top Gear series.
Set the setting to Default, Low, Medium, or Max. Be warned, there's a
handful of games that will not boot if the setting is anything but Default.
In those cases, you can workaround it by changing it after the game starts,
as most games will react to the setting in real time, others might require
a virtual Reset.

• Sprites per-line Limit: when disabled, this will allow the emulated
console to break the original hardware limitation of 32 sprites per-scanline
limit, so sprites don't dissappear or flicker. Specially useful for games
that show lots of sprites on screen (i.e.: Gradius III, BioMetal, etc).

• Satellaview BIOS: when disabled, this will boot the BS-X games directly
through the emulated console. The reason why this is an option, is because
not every Satellaview game has been correctly dumped yet, and some work
only by disabling the add-on, as the BIOS doesn't recognize the ROM
correctly due to the missing bits of data.
```


## MSU-1 CO-PROCESSOR

The MSU-1 is a custom coprocessor that sits inside the game cartridge,
not entirely unlike the Super FX, SDD-1, CX4, SA-1 or the DSP series, used
in games such as Doom, Star Ocean, Mega Man X2, Kirby's Dream Land 3,
or Top Gear 3000, respectively. This expansion chip was designed by byuu
(later known as Near), the author of bsnes and higan, the most accurate to
hardware, Super Nintendo / Super Famicom emulators ever made.

The enhancement chip enables playback of CD-quality audio (uncompressed
16-bit PCM at 44,100 kHz), along with full-motion video, and even the
streaming of new graphic frames into games. Another neat trick is to
store program data on it, copy this data into the SNES main RAM and
execute it from there. All of this is possible as the MSU-1 addresses
up to 4GB of data, far more than a typical SNES cartridge could ever hold.


## SATELLAVIEW (BS-X)

To emulate the St. GIGA's satellite service, some of its exclusive games
require the obligated use of the add-on's BIOS. You're free to use the
japanese BIOS file, or the recommended english translated (No DRM) version.

The correct values for the file (English+No DRM, version 1.3) are:
Size: 1.048.576 bytes
CRC32: E5A91AD4
MD5: 96CF17BF589FCBFA6F8DE2DC84F19FA2
SHA-1: 4891D739A8A8B67923681BAD4FB67EDAB2E90E50

Rename the file and its extension to "BS-X.BIN", then put it inside
the "snes9xgx" folder at the root of the device. (SD or USB)

Though the BIOS use is optional, it is required for a bunch of the
titles, but specially, for the digital magazines.

If you need a place to get the correct file, check the Links section
down below, and visit the BS-X Project website.


## USB CONTROLLERS

To enable the Speedlink Hornet Gamepad or the Xbox 360 (wired) controller,
there are two ways available:

Before loading Snes9x RX, connect your Xbox 360 wired controller. If the
other USB port is populated (example: USB HDD, flash drive, DualShock 3)
it should work the moment you start a game. For manual detection, when
you're at the main screen (Choose Game), click on the emulator logo at
the corner and check the status info at the bottom, to confirm detection.
The same can be achieved by opening the Credits section inside "Settings".

Remember, the controller only works when in-game. You can swap your
player/port number by simply pressing on the Xbox Guide button.

To enable the DualShock 3 (wired) controller, press and hold both
minus (-) and plus (+) buttons in sequence, then release. You
can do this in the Wiimote, or even the Wii U Pro Controller.
The DS3 led #1 should light up once, and then the four leds.
After that, press the PS button, it should be enabled for in-game use
by now. You can do this before loading any game, for example.


## TURBO MODE

Turbo Mode increases the playback speed of the game by about 2x. By default,
to use it simply press and hold right on the 'C-stick' (yellow control stick
on the Gamecube controller) or the right analog stick on the Wii Classic
Controller / Wii Classic Controller Pro / Wii U Pro Controller for as long
as you want gameplay to be faster. Release the stick/button whenever you
want normal playback speed to resume.

Remember that this function can be disabled or remapped to other buttons
inside the Game Menu (Game Settings -> Button Mappings -> Other Mappings).


## IMPORTING AND EXPORTING SRAM

Snes9x RX includes the ability to load SRAM save files created with Snes9x
version 1.52 and onwards on other platforms (Mac/PC/Linux/etc.), and to use
the save file back to those.

To load a SRAM file on the Gamecube / Wii / Wii U from another platform,
ensure the name of the new .SRM file matches the filename of the ROM on
your device.

To use a Snes9x RX SRAM file on another platform, just do the opposite: 
copy the saved SRAM file to the other platform. You may have to rename the 
file or the extension to be what that version of Snes9x expects it to be,
like .SRM to .SAV, for example.


## AUTOBOOT MODE

Snes9x RX also sports an autoboot feature, for special use with custom
forwarders made to look like Wii Virtual Console channels, or individual
entries on your Homebrew Channel. To make use of this feature, just add
the following lines to your meta.xml right between ```</long_description>```
and ```</app>```, like the following example:

```
   </long_description>
   <arguments>
   <arg>sd:/snes9xgx/roms</arg>
   <arg>game.sfc</arg>
   </arguments>
   <ahb_access/>
 </app>
```

Use "sd:" OR "usb:" according to your media, adjust the path to the specific
location of the ROM on your device, and replace "game.sfc" with the specific
name of your game file (can be a .zip, too).

Make sure to set your configuration to your liking before using autoboot,
as you won't be able to change the ones that are only accesible inside the
Settings menu at the emulator's Main Menu / Game browser.


## UPDATE HISTORY

[5.4.0 - October 15, 2022]
* Map YXBA to Right Stick (thanks InfiniteBlueGX!)
Right stick can now be configured as YXBA, like what the Xbox 360 wired
controller is configured by default with this emulator, specially useful
for shooters like Smash TV and Total Carnage.

* Add option to choose the Emulator Menu toggle [InfiniteBlueGX]
Choose between "Default (All Enabled)", "Home / C-Stick Left", or
the universal button combo "Start+B+A / Start+1+2".

* UI navigation improvements. [InfiniteBlueGX]
Pressing B / 1 will now Go Back from all menus and some sub-menus.

* Satellaview BIOS ON-OFF (thanks Tanooki16!)
In RX, it was changed and adapted to be intuitive and easy to use.
Enable or disable BS-X Satellaview BIOS boot through:
"Settings -> Menu" or "Game Settings -> Emulator Hacks".

[5.3.0 - September 28, 2022]
* Upgraded Satellaview (BS-X) engine to latest Snes9x to date.
This furthers up the game compatibility, by making use of the Satellaview
BIOS. Though the file is optional, you'll want to use it for titles that
make exclusive use of its functions. Some of the titles now playable are:
- BS Fire Emblem: Akaneia Saga (Episodes 1 to 4)
- Chou Aniki - Bakuretsu Rantou Hen
- Konae-chan no Dokidoki Penguin Kazoku Event-ban

And a lot of the digital magazines available that were distributed through
the Satellite's service can be read in its original language now,
as the BIOS embedded font is mostly used for these.

Check the instructions on where to place the BIOS file by reading the new
Satellaview section down below, here in the readme.

* MSU-1 refinements.
* Fix for compiling error.
* Updates for the Spanish language.
* Other tweaks.

[5.2.0 - June 18, 2022]
* SNES CPU overclock setting exposed (thanks Tanooki16!)
Inside the "Video" section, you can now choose three settings to overclock
the virtual SNES CPU, to improve or smooth the framerate in games that
originally struggled (i.e.: cutscenes in Flashback). It may also change the
flow of the game entirely (i.e.: Skulljagger - Revolt of the Westicans).
Experiment with the setting on your favorite games or other uncommon titles
in your library.
* Updates for the Spanish language.
* Other tweaks.

[5.1.0 - June 26, 2022]
* Reset settings if an older config file is found
Preferences XML file will be reset if it is older than 5.1.0, in order to
start clean and avoid possible conflicts.
* Korean language update, minor cleanup. [DDinghoya]
* Remove unused logger.cpp and logger.h. [bladeoner]
* Fix the logic for the Display Virtual Memory toggle. [InfiniteBlueGX]
* Cleanups backported from the Libretro cores.
* dsp: Fix assignment of Op11Xr. [jonathan-teh]
* apu/dsp: Mark function-scope const arrays as static. [jSTE0]
* Fix some memory leaks. [jdgleaver]
* Remove OpenGL options. Not needed here.
* Remap Turbo Mode and add a submenu. (thanks InfiniteBlueGX!)
* Fix an edge case where Turbo Mode could be activated on Dpad Up/Left
when Nunchuk's Z/C button is mapped. [InfiniteBlueGX]
* Some renaming for TurboMode. [InfiniteBlueGX]
* Add an enumeration for the remappable buttons
for Turbo Mode. [InfiniteBlueGX]
* SuperFX OC value will properly load on next boot. [InfiniteBlueGX]
* Fix some formatting. [InfiniteBlueGX]
* Add a toggle to hide/show the SRAM save button
in the save menu UI. [InfiniteBlueGX]
* Remove an unused variable? [InfiniteBlueGX]
* New audio filters (CUBIC/SINC) taken from Snes9x 1.61.
* Invert L/R audio channels, save more settings. [Tanooki16]
You can now swap Left and Right audio channels with a toggle.
* New speeds for Super FX overclocking, Wii U recommended.
Added 80 MHz / 100 MHz / 120 MHz. These will stay hidden on the
Gamecube port's GUI, as the CPU is not powerful enough.
* SNES Hi-Res Mode ON/OFF and Sprite Limit ON/OFF (thanks Tanooki16!)
* Important readme updates.
* Updates for the Spanish language.
* Other tweaks.

[5.0.0 - Abril 22, 2022]
* Use I4 instead of RGBA8 for fonts (much less memory). [Daryl]
* When unable to load the default rom directory, just drop into device
root. Don't show an error when unable to find a load device. [Daryl]
* Silence a few warnings. [Daryl]
* Remove S9xChooseMovieFilename. [bearoso]
* Remove S9xSetPalette. [bearoso]
* Remove S9xChooseFilename. [bearoso]
This is integration of the frontend with the core. Disable
the snapshot button mappings that use it. Any frontend should
implement those port commands its own.
* Load cover images directly from file instead of an
intermediary buffer. [Daryl]
* Correct aspect ratio by changing viWidth to 644. [vaguerant]
* Add ability to change the player mapped to a
connected (Wireless) controller. [Tantric]
* Change max game image dimensions to 640x480, fix bug
in png loading. [Tantric]
* Add support for Mayflash 2-port PC044 SNES USB adapter. [EthanArmbrust]
* New scanlines filter setting. (thanks Tanooki16!)
Now nicknamed 50% and 25% for RX, I added the option to select between both,
so you can choose whether you like darker scanlines (old method)
or subtler ones (new method).
* Add A+B+SELECT+START for back to menu on Wiimote controller extensions.
Based on the similar commit by Tantric for Snes9xGX.
* If arguments are passed to the emu to autoboot a game, then the main
menu button should be labelled Exit, and leave the emu instead of going
back to the main menu. Cleanup autoboot code. [Tantric]
* Add support for mapping more than 128KByte SRAM. [cout/qwertymodo]
* Add 128KByte SRAM support in cheats. [qwertymodo]
* New Scale2x filter added. (thanks Tanooki16!)
Originally developed by Andrea Mazzoleni for the AdvanceMAME project.
http://www.scale2x.it/
* Add support for Speedlink Hornet Gamepad USB. (thanks revvv!)
* Prevent cheat name overflow. [Daryl]
* Support forwarders that pass in sd1:/ [Tantric]
* Add ability of FastROM hacks to use SuperFX. [bladeoner]
* Set SRAM initialization to set whole buffer. [bearoso]
...not just a few bytes. Add a TODO comment at allocation.
These never change, so they should ideally be static.
* Add heuristic to detect 6MB Earthbound hack.
Makes "Mother 2 Deluxe" romhack playable.
* UStealth support.
* Wii 480p video fix. [Extrems]
* More 3rd party controllers support. [Tantric]
Fix 3rd party classic controllers that don't send calibration data.
For those controllers, use default values.
* Important readme updates.

[4.9.0 - July 15, 2020]
* Reduce save buffer size on GCN. Should fix preview glitch. [Tantric]
* Snes9x - Increase SRAM size to 512KB. [cout]
* Wii U widescreen patch, report whether Wii U CPU is full speed. [Daryl]
Use the Credits section to see it (press the Snes9xRX logo on the main menu)
* Fix some warnings. [bearoso]

[4.8.0 - March 10, 2020]
* Language updates for Spanish, French, Portuguese.
* .bs file extension support.
* Classify region id 18 as PAL. [Tantric]
* Set default calibration values, fix controllers that return invalid data.
* Quick fixes for Rendering Ranger R2 and Targa (50/60Hz).

[4.7.0 - February 02, 2020]
* Kirby Super Star GCN performance fix.
30+ FPS boost for this game, should make it enjoyable again on the Cube.
* Add Show Local Time option. [bladeoner/Tantric]
* Optimize USB controllers handling. [revvv]
Only open device if VID+PID match.
* ios version up [revvv]
* GCN build fixes (thanks emukidid!)
* Revamped README.
* Create missing folders.
In case one or more of the "\snes9xgx" folders are absent, they will be
created on the second run of the emulator, after a settingsRX.xml has been
generated by pressing Exit on first run.

* Experimental DualShock 3 (wired) support.
Based on libsickaxis 1.0 by Xerpi. As of now, it controls the 2-4 players
at the same time. Could and should be upgraded in the future to polish up
this implementation, any help on this task will be welcome.

[4.6.0 - December 24, 2019]
* Minor cosmetic tweaks.
* Retrode 2 code cleanup.
* Xbox 360 Controller code cleanup.
* LED fix for different X360 Controller revision.
* Fix GCN build.

Now available in various skins/colors, choose the one you like the most:
* Cosmo Black (Default)
* SNS Mini Edition (USA)
* Midnight Purple
* Aqua Blue
* SNS Mini Edition (EUR)

[4.5.0 - November 22, 2019]
* Xbox 360 wired controller support! (thanks revvv!)
Before loading Snes9x RX, connect your Xbox 360 wired controller. When
you're at the main screen (Choose a game), click on the emulator logo at the
corner of the screen and read the status info at the bottom, just to make
sure it was properly detected. In some cases you won't need to do this,
it will just work. Remember, the controller only works when in-game.
You can swap your player/port number by simply pressing on the
Xbox Guide button. Enjoy!

Right stick is configured as YXBA (essentially duplicating your buttons),
specially useful for Smash TV fans like me =D

* Xbox 360 wired controller code improvements. [revvv]

[4.4.0 - November 07, 2019]
* Fixed Funaki Masakatsu Hybrid Wrestler – Tougi Denshou graphical glitch.
* Retrode 2 support tweaks.

[4.3.0 - August 14, 2019]
* Fixed "PowerFest 94 - Super Mario Kart" black screen.
* Fixed Kat's Run - Zen-Nihon K-Car Senshuken graphic bg corruption during
demo. Phalanx random black screen is fixed too.
* Fixed Clayfighter blue clown face when selecting a player.
* Fixed Stunt Race FX graphical glitch on the course selection screen.
* Fixed Light Fantasy SRAM saving issues.
* Fix out-of-bounds memory access. [bearoso]
* Working buttons for all SNES peripherals.
Mouse, SuperScope and the Konami's Justifier trigger/buttons never worked in
any other controllers except the GCN pad and Wiimote. Now you can use the
Wii Classic Controller, Wii U Pro Controller and Wii U Gamepad to
fully emulate the peripherals.

[4.2.0 - August 07, 2019]
* Avoid USB call if there's no Retrode. [revvv]
* Fix M.A.C.S. Basic Rifle Marksmanship. [ghost - OV2]
The flickering was because game thinks joypad2 is constantly firing on/off.
* Cleanup time.
* Spanish language translation update.
* JoJo no Kimyō na Bōken and Kick Off graphical glitches fixed. [bearoso]
* Fixed Speedy Gonzales - Los Gatos Bandidos game freeze. [bearoso]
* Fixed Doom graphical garbage. [twinaphex]

[4.1.0 - August 01, 2019]
* Backport+adjust the refactored APU Resampler. [bladeoner]
* Adjust default input rate.
* Retrode 2 USB adapter support (thank revvv!)
The Retrode 2 cartridge reader offers USB mass storage access for your SNES
cartridges, besides 4 ports for original controllers, more specifically:
two SuperNES and two Genesis gamepads. 2 players are supported!

Some notes from revvv:
"- If the Retrode does not react, you just have to restart Snes9x GX.
I never had to restart HBC or the Wii. This happens with my fork, too.
But not very often.
- Doom is a good testcase: My first build had a huge lag, but only with
this game. After polling the Retrode only for player 1, the lag disappeared.
(Doom is a single player game, so it's strange that they poll player 2.)"

[4.0.0 - July 28, 2019]
* Add Wii U GamePad support. [Fix94 - Tantric]
* Allow "Original" render mode to be selectable when using the Wii Options
TV Resolution setting for "EDTV or HDTV (480p)" over component cables:
- This caters specifically to LCD / LED users with 240p supported displays,
since the option was previously hidden. Users with CRT / PVM / BVM displays
with supported 480p Progressive Scan mode will also benefit, since no Wii
setting change will be needed for the "Original" 240p mode to be used.
* Restore MSU1 playback position correctly. [bearoso]
* Restore MSU1_AUDIO_POS. [bearoso]

[3.9.0 - July 26, 2019]
* Korean language update, minor cleanup. [DDinghoya]
* GFX.DoInterlace-- should occur even if we don't render frame. [bearoso]
* Move interlace flags to S9xSoftResetPPU. [bearoso]
* Fix PPU blending with unoptimized change. [bearoso]
* Use a lookup table. A little faster. [bearoso]
* Fix color add for non-GFX_MULTI_FORMAT. [bearoso]
* Make blending work with RGB555. [bearoso]
* Proper 16-bit color conversion. [bearoso]
* Use for loops for DRAW_TILE. 3-4% speed benefit. [bearoso]

[3.8.0 - July 24, 2019]
* Cleanup screenshot memory management. This fixes the preview image
not displaying on Gamecube. [Tantric]
* Tenshi No Uta (Japan) compatibility hack.

[3.7.0 - March 19, 2019]
* Fix issue with on-screen keyboard. [Tantric]
* Fix crash on launch when using network shares. [Tantric]
* Various settings fixes.
* Updated spanish language translation.

[3.6.0 - February 21, 2019]
* Remove wiiupc since libogc wiiuse supports WiiU Pro controller. [Tantric]
* Re-add explicit Wii U Pro controller mappings. [Tantric]
* Fix joystick calculations and controllers with no analog sticks. [Tantric]
* Simplify logic for controller analog sticks. [Tantric]
* Fix crash for Wiiflow plugin mode. (thanks, fledge68!)

[3.5.0 - February 02, 2019]
* Add Interpolation option and add Gamemenu Audio. [bladeoner]
This adds the following:
- A new "Audio" menu inside "Game". Now you can choose between:
Gaussian Interpolation (Accurate), Linear, or None.
* Restore GUI sounds and BG music.
* Add ability to externally load fonts and activate Japanese/Korean. [Tantric]
Put the jp.ttf and ko.ttf inside the Apps > Snes9xRX folder.
You can download them from the Snes9X RX GitHub "hbc" folder.
* Add support to load external background music. [Tantric]
Put your bg_music.ogg inside the Apps > Snes9xRX folder.

[3.4.0 - February 01, 2019]
* Quick and dirty attempt to prevent reading and writing
from/to the same audio buffer. [Tantric]
* Avoid using file stat when possible. It's slow. [Tantric]
* Fixed black screen: Tengai Makyou Zero. [bladeoner]

[3.3.0 - January 28, 2019]
* Remove two asserts in SPC.
* Rewritten audio code. WIP. [Tantric]
* Add logic to update the playback rate dynamically. [Tantric]

[3.2.0 - January 26, 2019]
* We only use the HermiteResampler. [Tantric]
* SwitchAudioMode update.
* Update hermite resampler to support dynamic rate control.
Fixes audio blips. Remove some asserts in APU. [Tantric]

[3.1.0 - January 24, 2019]
* Kirby Super Star intro fix. (thanks, bladeoner!)
* Reorder init to init snes9x memory earlier so it goes into MEM1. [Tantric]
* Mute sound when in turbo mode, otherwise the APU buffer can get messed up. [Tantric]
* Fix sound crackling. [Tantric]
* Change audio playback to 48khz. this should fix the tinny sound problem. [Tantric]
* Try to improve audio sync & reduce sound input rate slightly. [Tantric]
* Disable sound sync (if enabled) when using turbo mode.
Fixes sound cutting off when using turbo. [Tantric]
* Also break out of S9xMainLoop in original location. [bearoso]
* Invoke Menu with Start+A+B+Z, special for NES-SNES to GCN adapters.

[3.0.0 - January 08, 2019]
* Gamecube Virtual Memory implementation. [emukidid]
- Adds ARAM usage via the TLB.
* Add toggle to enable/disable virtual memory info.
* Miscellaneous fixes.

[2.9.0 - January 07, 2019]
* Port option to not append "Auto" from vbagx. [libertyernie]
* Correct the default aspect ratio if the Wii has 16:9 set up. [Tantric]

[2.8.0 - January 06, 2019]
* Credits crash fix and minor update.
* Removed ImageFolder from GCSettings because it can always be retrieved
from GCSettings.PreviewImage, added function to get its value. [cebolleto]
* Changing image preview with plus button. [cebolleto]

[2.7.0 - January 03, 2019]
* Remove GUI Sounds and BG Music. A bit more resources available now. [bladeoner]
* Change settings.xml to settingsRX.xml [bladeoner]
* Remove rumble in GUI function. [bladeoner]
* Rollback scanline filter fix. Makes it crash when loading a ROM on the GCN port.
* Backport fix GC build with scanline filter. [Tantric - bladeoner]
* Forgotten cleanup for remove rumble function. [bladeoner]

[2.6.0 - December 29, 2018]
* Settings saving fix. (thanks, Askot!)
* New video filters / Fix for HQ2X-Scanlines change. [Tantric]
* Minor menu optimizations. [Tantric]
* Rollback graphic fix that broke StarFox graphics.

[2.5.0 - December 24, 2018]
* Remove some debugger code in cpuexec.
* Fix Mario's Time Machine. [bearoso]
* Fix tile selection in mosaic offset-per-tile mode. Fixes first Contra 3 boss. [bearoso]

[2.4.0 - December 22, 2018]
* Use a license stub everywhere. [bladeoner]

[2.3.0 - December 20, 2018]
* Remove some debugger code.
* Remove some movie code from logger.
* Change where we break S9xMainLoopScan for input (Brunnis lag fix) [bearoso]
* Don't break interlace syncopation on frame skip. [bearoso]
* Add DMA timing hack for Koryu no Mimi translation by rpgone. [OV2]

[2.2.0 - December 7, 2018]
* Update ko.lang [DDinghoya]
* Automatically create preview image dirs if they don't exist. [Tantric]
* Remove update check completely. [Tantric]
* Reorder init to init snes9x memory earlier so it goes into MEM1. [Tantric]
* Disable multi pixel format support. [Tantric]
* Code cleanup and fix include references. [bladeoner]
* Change some defaults ("Artworks" to "Artwork"). [Tantric]
* Prevent overrunning the file buffer, increase buffer size to load larger IPS/UPS files. [Tantric]

[2.1.0 - November 26, 2018]
* Add BPS soft-patching support. [qwertymodo]
* MSU1 fixes backported. [bladeoner, qwertymodo]
* Compile fixes for Linux. [bladeoner]
* Allow loader (e.g. Homebrew Channel) to pass two arguments instead of three for autoload. [libertyernie]
* Check argc. [libertyernie]

[2.0.0 - October 21, 2017]
* Compatible with the new english translation for "Tengai Makyou Zero - FeoE".

[1.9.0 - October 10, 2017]
* Remove things and tidy up.

[1.8.0 - September 29, 2017]
* Partially remove movie code (part 6).
* Update mouse handling.
* Partially remove NETPLAY code.

[1.7.2 - September 27, 2017]
* Partially remove movie code (part 5).

[1.7.1 - September 26, 2017]
* Partially remove movie code (part 4).

[1.7.0 - September 25, 2017]
* Partially remove movie code (part 3).

[1.6.0 - September 05, 2017]
* Partially remove movie code (part 2).
* Fix MSU-1 file loading after saving/loading snapshots. [qwertymodo]
* Sync MSU-1 code with upstream (sync 2). [qwertymodo]

[1.5.0 - September 01, 2017]
* Partially remove movie code (part 1).
* New attempt to fix RAM mapping for Light Fantasy (matches Higan). [qwertymodo]

[1.4.0 - August 31, 2017]
* SuperFX fixes and improvements, some from snes9x2010. [jamsilva]

[1.3.0 - August 30, 2017]
* Added 20 MHz overclock option for the SuperFX chip.
* Remove movie code. [twinaphex]
* Sync MSU-1 code with upstream (sync 1). [qwertymodo]
* Circuit USA timing hack. [bearoso]

[1.2.0 - July 03, 2017]
* Copied VLDC9 fix from snes9x_3ds. [jamsilva]
* Support for more SA1 char conversion modes. [jamsilva]
* Still cleaning things up...  [jamsilva]

[1.1.0 - January 14, 2017]
* Remove unnecessary msu1 reset. [OV2]
* Pack status registers before snapshotting so they're not lost. [GregorR]

[1.0.0 - December 27, 2016]

* New color scheme.
* Changed references to bapu/dsp
* Revisited and updated spanish translation.
* Revisited and updated italian translation.
* Removed unused files.
* Fixed GC build.
* Fast-Forward on the right stick is enabled again.
* MSU-1 fixes from the qwertymodo branch.
* The minimum file size for a ROM is now 30KB.
* Fixed typos.


## UPDATE HISTORY (PRE-RX)

[4.3.7 - December 9, 2016]

* Hide saving dialog that pops up briefly when returning from a game

[4.3.6 - September 12, 2016]

* Added the delete save file (SRAM / Snapshot) option
* Changed the box colors for the SRAM and Snapshots files to match the color scheme of the emu GUI
* Change the "Power off Wii" exit option to completely turn off the wii, ignoring the WC24 settings
* Updated emulator credits
* Added an option to switch between screenshots, covers, or artworks images,
  with their respectively named folders inside /snes9xgx at the device's root.
  You can set which one to show, by going to Settings > Menu > Preview Image.
  The .PNG image file needs to have the same name as the ROM (e.g.: Contra III.png)

[4.3.5 - February 06, 2016]

* Added Fix94 wiiflow plugin mode
* Removed sound from GUI and now gets better perfomance/FPS on games like 
  Yoshi's Island and Kirby Dream Land 3.

[4.3.4 - February 2, 2016]

* Fixed screenshot image dimensions
* Fixed screenshot option, it no longer creates an additional "dummy" file
* Fixed performance issues, reverted to previous vsync method
* Removed automatic download of newer versions by Burnt Lasagna.
* Compiled with devkitPPC r26
  Note: If compiled with devkitPPC r27 some games, like Final Fantasy III
	and Chrono Trigger would crash on a battle

[4.3.3 - September 3, 2015 - July 7, 2015]

* Added Cebolleto's preview image support
* Added WiiUPro controller support
* Added a Scanline filter option
* Increase preview image size and reduce game list width
* Added a background to the preview image
* Added a Screenshot button
* Added a "WiiuPro" button on the button mapping menu
* Fixed the inverted color button selection that was in some option windows

[4.3.2 - November 9, 2012]

* Fixed lag with GameCube controllers

[4.3.1 - July 7, 2012]

* Fixed PAL support

[4.3.0 - July 6, 2012]

* Support for newer Wiimotes
* Fixed screen flicker when going back to menu
* Improved L/R buttons for GameCube - trigger button press when 50%+ depressed
* Improved controller behavior - allow two directions to be pressed simultaneously
* Timing changes
* Compiled with devkitPPC r26 and libogc 1.8.11

[4.2.9 - January 14, 2012]

* More accurate pixel scaling (thanks eke-eke!)
* Other minor changes

[4.2.8 - May 15, 2011]

* Ported a few upstream game fixes for: Mutant Chronicles - Doom Troopers, 
  Porky Pig's Haunted Holiday, Big Sky Trooper, and Mechwarrior 3050 / Battle 
  Tech 3050
* Added Turkish translation

[4.2.7 - March 23, 2011]

* Fixed browser regressions with stability and speed
* Reverted zones' changes to IRQ and SA-1 - these caused a performance hit

[4.2.6 - March 19, 2011]

* Improved game compatibility (updated core to latest Snes9x)
* Fixed issue with cheats not persisting
* Improved USB and controller compatibility (recompiled with latest libogc)
* Enabled SMB on GameCube (thanks Extrems!)
* Added Catalan translation
* Translation updates

[4.2.5 - October 7, 2010]

* Sync with upstream SVN - fixes a few specific game issues
* Fixed "blank listing" issue for SMB
* Improved USB compatibility and speed
* Added Portuguese and Brazilian Portuguese translations
* Other minor changes

[4.2.4 - August 14, 2010]

* IOS 202 support removed
* USB 2.0 support via IOS 58 added - requires that IOS58 be pre-installed
* DVD support via AHBPROT - requires latest HBC

[4.2.3 - July 22, 2010]

* Fixed broken auto-update

[4.2.2 - July 20, 2010]

* Reverted USB2 changes
* Fixed return-to-menu crash with Filtered mode

[4.2.1 - July 14, 2010]

* Improved audio timing
* Fixed 16:9 correction in Original mode
* Ability to use both USB ports (requires updated IOS 202 - WARNING: older 
  versions of IOS 202 are NO LONGER supported)
* Fixed issue with IPS patch files
* Hide non-ROM files
* Other minor improvements

[4.2.0 - June 20, 2010]

* Fixed incorrect aspect ratio issue
* Fixed choppy framerate issue
* Fixed IPS/UPS patching
* USB improvements
* GameCube improvements - audio, SD Gecko, show thumbnails for saves
* Other minor changes

[4.1.9 - May 19, 2010]

* DVD support fixed
* Fixed some cheats issues
* Fixed some potential hangs when returning to menu
* Video/audio code changes
* Fixed scrolling text bug
* Other minor changes

[4.1.8 - April 9, 2010]

* Fix auto-save bug

[4.1.7 - April 9, 2010]

* Freezing issue fixed
* Core timing fixes, should solve some problems with some games
* Most 3rd party controllers should work now (you're welcome!)
* 7z crash fixed
* GameCube only - DVD/SD Gecko fixed (thanks emukidid!)
* Translation updates (German and Dutch)
* Other minor changes

[4.1.6 - March 30, 2010]

* New core! Updated to Snes9x 1.52. Old save states will not work!
* DVD / USB 2.0 support via IOS 202. DVDx support has been dropped. It is
  highly recommended to install IOS 202 via the included installer
* Multi-language support (only French translation is fully complete)
* Thank you to everyone who submitted translations
* SMB improvements/bug fixes
* Minor video & input performance optimizations
* Now uses .srm files without "Auto" appended, if found
* Added option to disable crosshair

[4.1.5 - December 23, 2009]

* Changed default folders to snes9xgx/roms and snes9xgx/saves. Old folders
  will be automatically moved to the new location
* File browser now scrolls down to the last game when returning to browser
* Auto update for those using USB now works
* Fixed scrollbar up/down buttons
* Minor optimizations

[4.1.4 - December 2, 2009]

* Fixed SMB (for real this time!)
* Fixed snapshot loading regression

[4.1.3 - November 30, 2009]

* Fixed SMB
* Added separate horizontal/vertical zoom options
* Improved scrolling timing - the more you scroll, the fast it goes
* Fixed reset button on Wii console - now you can reset multiple times
* Minor code optimizations
* Reduce memory fragmentation - fixes out of memory crashes

[4.1.2 - October 7, 2009]

* Revamped filebrowser and file I/O
* Many, many other bug fixes

[4.1.1 - September 19, 2009]

* Fixed black screen bug

[4.1.0 - September 16, 2009]

* Text rendering corrections
* SMB improvements
* Built with latest libraries
* Video mode switching now works properly
* Other minor bugfixes and cleanup

[4.0.9 - July 22, 2009]

* Fixed "No game saves found." message when there are actually saves.
* Fixed shift key on keyboard
* Text scrolling works again
* Change default prompt window selection to "Cancel" button

[4.0.8 - July 9, 2009]

* Faster SMB/USB browsing
* Last browsed folder is now remembered
* Fixed controller mapping reset button
* Fixed no sound on GameCube version
* Directory names are no longer altered
* Preferences now only saved on exit
* Fixed on-screen keyboard glitches
* SRAM auto-saved on power-off from within a game
* Prevent 7z lockups, better 7z error messages
* Increase cheats limit from 30 to 150
* Cheats no longer effect next game loaded - they are cleared properly

[4.0.7 - June 30, 2009]

* Fixed auto-update
* Increased file browser listing to 10 entries, decreased font size
* Added text scrolling on file browser
* Added reset button for controller mappings
* Settings are now loaded from USB when loading the app from USB on HBC
* Fixed menu crashes caused by ogg player bugs
* Fixed memory card saving verification bug
* Fixed game savebrowser bugs
* Miscellaneous code cleanup/corrections

[4.0.6 - May 30, 2009]

* Fixed SD/USB corruption bug
* SMB works again
* GUI bugs fixed, GUI behavioral improvements

[4.0.5 - May 26, 2009]

* Improved stability
* Fixed broken SDHC from HBC 1.0.2 update
* Fixed issues with returning to menu from in-game
* Add option to disable rumble
* Auto-determines if HBC is present - returns to Wii menu otherwise
* Fixed Super Scope turbo button issue
* Miscellaneous bugfixes

[4.0.4 - April 30, 2009]

* Improved scrollbar
* Built with more stable libogc/libfat
* Fixed rumble bug in filebrowser
* Added confirmation prompts
* Fixed settings saving glitches

[4.0.3 - April 23, 2009]

* Settings resetting glitch fixed

[4.0.2 - April 22, 2009]

* GameCube controller home trigger fixed
* USB support fixed
* More stable SMB support
* Corrections/improvements to game saving/loading
* Video mode corrections
* hq2x filter no longer crashes hi-res games on unfiltered/filtered modes
* Corrections to cheat file parsing
* Super Scope turbo now activated when holding Down button
* Settings are now saved when exiting game menu settings area
* Super Scope pause button now works
* Invalid VRAM access is now allowed - should fix some homebrew games
* New video mode selection in menu (forcing a video mode is not recommended)

[4.0.1 - April 13, 2009]

* Fixed turning off autosave in menu
* Keyboard fixed, more keys added
* Fixed 7z loading from DVD
* Enable auto loading and renaming of SRAM save without "Auto" in the name
* PAL resolution fixed - no more letterboxing
* File browser scrollbar box now draggable, arrow buttons now scroll list
* Better handling of multiple on-screen wiimotes
* Menu restructured - new "Game Settings" menu

[4.0.0 - April 4, 2009]

* New GX-based menu, with a completely redesigned layout. Has Wiimote IR 
  support, sounds, graphics, animation effects, and more
* Thanks to the3seashells for designing some top-notch artwork, to 
  Peter de Man for composing the music, and a special thanks to shagkur for 
  fixing libogc bugs that would have otherwise prevented the release
* Onscreen keyboard for changing save/load folders and network settings
* Menu configuration options (configurable exit button, wiimote orientation,
  volumes)
* Configurable button mapping for superscope, mouse and justifier
* New save manager, allowing multiple saves and save browsing. Shows
  screenshots for Snapshot saves, and save dates/times
* Experimental hq2x filter, contributed by michniewski

[009 - January 27, 2009]

* Faster SD/USB - new read-ahead cache
* Removed trigger of back to menu for Classic Controller right joystick
* Fixed a bug with reading files < 2048 bytes
* Fixed some memory leaks, buffer overflows, etc
* Code cleanup, other general bugfixes

[008 - December 24, 2008]

* Fixed unstable SD card access
* Proper SD/USB hotswap (Wii only)
* Auto-update feature (Wii only)
* Rewritten SMB access - speed boost, NTLM now supported (Wii only)
* Improved file access code
* Resetting preferences now resets controls
* Fixed "invalid file size" error on smaller games (eg: Space Invaders)
* Fixed hangup in Super Mario RPG
* Minor bug fixes

[007 - November 19, 2008]

* added: SDHC support
* added: SD/USB hot-swapping
* added: zoom saving
* added: IPS/UPS/PPF patch support
* added: Qoob modchip support (thanks emukidid!)
* added: Added console/remote power button support (Wii only)
* added: Added reset button support - resets game (Wii only)
* changed: Settings file is now named settingsRX.xml and is stored in the same
           folder as the DOL - eg: apps/Snes9xGX/settingsRX.xml (Wii only)
* fixed: swc, sfc file support
* fixed: inverted sound channels
* fixed: some game crashes
* fixed: snapshot saving for games with SPC7110, BS, DSP, or CX4
* fixed: justifier support
* fixed: superscope turbo button
* fixed: widescreen support
* fixed: ActRaiser 2 issues
* fixed: Invalid memory accesses in C4 and OBC1. MMX3 Toxic Seahorse stage
         now can be emulated with HDMA. (zones)
* fixed: Updated snapshot to prevent desync. Added some variables related to
         APU and HDMA. (gocha)
* fixed: zoom issues (thanks eke-eke!)
* fixed: original modes (thanks eke-eke!)
* fixed: vertical scaling for filtered/unfiltered modes (thanks eke-eke!)

[006 - October 15, 2008]

Tantric
* added: 480p for GameCube
* added: Sound sync
* added: 7z support
* changed: Faster SD/USB access (readahead cache enabled)
* fixed: Video offset issues
* fixed: BS-X games work now
* fixed: Wii DVD works now
* fixed: DVD re-enabled for GameCube
* fixed: Nunchuk analog stick issues
* fixed: Many crashes, memory leaks, etc

michniewski
* added: Video shift options
* changed: Turn DVD motor off option re-enabled for GameCube

[005 - September 23, 2008]

michniewski
* added: Superscope/mouse/justifier support, with Wii remote
* added: 3 render modes - Original, Filtered, Unfiltered
* added: widescreen compensation option
* added: DVD support on the Wii
* changed: zoom - limited range, added reset zoom option

Tantric
* added: now uses SNES 1.51 core (thanks to eke-eke for help with this)
* added: cheats menu! Loads .CHT file from /snes9x/cheats folder, 
         .CHT file name must match file name of ROM
* added: load/save preference selector. ROM, SRAM, Freeze, and preferences 
         are saved/loaded according to these
* added: preliminary Windows file share loading/saving (SMB) support on Wii:
		 You can input your network settings into snes9xGX.xml, or edit 
		 s9xconfig.cpp from the source code and compile.
* added: 'Auto' settings for save/load - attempts to automatically determine
         your load/save device(s) - SD, USB, Memory Card, DVD, SMB
* added: ROM Information page
* added: Game Menu - all game-specific options are here now: 
         SRAM save/load, Snapshot save/load, game reload, etc
* added: Credits page
* fixed: sd gecko works now
* fixed: full USB support
* changed: menu structure
* changed: preferences are now loaded and saved in XML format. You can open
		   snes9xGX.xml edit all settings, including some not available within
		   the program
* changed: if Home button is pressed when a game is running, Game Menu pops up
* changed: if preferences can't be loaded at the start and/or are reset, 
           preferences menu pops up - remove to save your preferences!
* changed: SRAM load - game reloaded automatically after loading SRAM

[004 - August 5, 2008]

* added: option to disable AA filtering 
         (snes graphics 'crisper', AA now default OFF)
* added: mapped zooming and turbo mode to classic controller
* added: preliminary usb support (loading)
* changed: sram and freezes now saved by filename, not internal romname. 
           If you have multiple versions of the same game, you can now have 
           srams and freezes for each version. A prompt to convert to the 
           new naming is provided for sram only.
* changed: by default, autoload/save sram and freeze enabled

[003 - July 25, 2008]
* added: alphabetical file sorting
* added: background logo/backdrop + nicer menus
* added: scrolling in ROM selector
* fixed: switching between pal/ntsc ROMS doesn't mess up timings
* fixed: GC controller config works now
* fixed: freeze autoloading on ROM load
* fixed: zipped ROMS should now load in a reasonable time
* fixed: precompiled dols for autosaving to various locations (see readme)
* changed: GC default quickload slot (to sd) (thanks kerframil)
* changed: default load/save dirs are now "/snes9x/roms" and 
           "/snes9x/saves/"  (thanks kerframil)
* changed: Classic X and Y defaults aren't switched
* changed: if autosave is enabled, it doesn't ask to save SRAM 
           anymore. It is saved in the background.
* updated README

[002 - July 21, 2008]
* added: classic and nunchuk support
* added: all controllers can now be configured
* added: GC version (untested)
* changed: mappings are no longer stored in SRAM, but in config file. 
           This means no per-game configurations, but one global 
           config per controller.
* one makefile to make all versions. (thanks to snes9x143 SVN)


[001 - July 12, 2008]
* compiles with latest devkitppc (r15)
* now uses libfat (can use front sd slot on wii)
* updated menu items a bit
* wiimote support
* fixed: autoload sram/freeze
* fixed: rom plays immediately after loading

[2.0.1b8]
* Added: SD slot B options for freezes, sram and loading of roms
* Changed: SMB options no longer displayed in menus when run on a Wii
* Changed: Game auto resumes running after resetting when choosing the "Reset
    Game" menu option
* Fixed (maybe): Reading of DVDs past the 1.36 GB barrier (Wii only) please
    test! - svpe

[2.0.1b7]
* Fixed: Zip compressed freezes to memory card could become corrupted as the
    file size changed - fixed this by deleting the existing file before writing
    a new one if the file size increased. If the file got smaller or stayed the
    same the original file is updated, using less of the existing file if the
    actual file size is smaller. A check is made before deleting the existing
    freeze file to ensure that there is enough space available for the new
    file. Note that additional space equivalent to the new file size must be
    available. If not enough space is available the original freeze is retained
    and the user is informed of the lack of space.
* Fixed: If option to auto-load freeze was selected, joypad config would not
    be restored since that is stored in SRAM. Resolved this for now by first
    loading SRAM if any and then loading the freeze. Obviously having to have
    both SRAM and freeze is not ideal, but this gets the job done if you have
    enough space on your memory card, SD card, etc.
* Added prompt when returning to the menu with autosave enabled allowing the
    user choose whether or not to perform the save. Press A to save or B if you
    don't wish to save.
* Added optional verification of Gamecube memory card saves. After writing
    the file it reads it back in and verifies that the written file matches
    what was to be saved. If it doesn't or if there was a problem opening the
    file it reports the problem to the user. Set this option in the preferences
    if desired.
* Added Reset Gamecube/Wii menu item
* Experimental DVD support for reading beyond 1.36 GB barrier on Wii. I have
    no way to test this, so please report on whether or not it works! Based on
    svpe's code.
    
NOTE: due to changes in the settings, this version will reset your emulator
options settings, so if you had saved preferences you will need to make your
changes to the emulator settings again and save them.

[2.0.1b6a]
* Fixed: Going up a directory when selecting a rom on a DVD wasn't working
    
[2.0.1b6]
* PAL Wii support - no separate version necessary! - eke-eke
* PAL roms now play at correct speed via internal timer, ntsc roms still use
    more accurate VSYNC timing - eke-eke
* Zipped freezes to memory card - take 9-12 blocks or so - based on denman's
    code
* Added option for auto save and load of freezes. For saving, can do both SRAM
    and Freeze if desired
* Memory card saving and loading shows a progress bar
* More miscellaneous ease-of-use improvements and cleanup
* Fixed: pressing B to get out of a rom file selection screen no longer drops
    you all the way back to the main menu. Now goes back to choice of where to
    load ROM (the "Load from DVD", "Load from SMB"... screen)
* Fixed: loading of joypad configuration in SRAM works again - no longer gets
    messed up

[2.0.1b5]
* B button implemented in all menus (returns to previous menu)
* Fixed bug when freezing state to SD card - would crash if SD support was not
    previously initialized
* Fixed double A button press needed after manual prefs/sram save to memory card
* Fixed delay after pressing A button after saving freeze to SD card
* Fixed problem of ".srm" SRAM file being created when SRAM was saved with no
    ROM loaded
* Fixed version number in SRAM and preferences
* Minor other code revisions

[2.0.1b1 through 2.0.1b4]
* SRAM saving and loading from snes9x on other platforms via SD card or SMB
* Games now autostart once loaded
* After manually loading SRAM the emulator is automatically reset
* Optional auto-loading of SRAM from memory card, SD or SMB after game loads
* Optional auto-saving of SRAM to memory card, SD or SMB when returning to menu
* TurboMode
* Global emulator preferences
* Menus redesigned (hopefully for the better!)
* Comes in 6 variants, each auto-loading/saving preferences/sram to a different
  location: mcslota, mcslotb, sdslota, sdslotb, smb, and noload
* ROM injector works again
* A number of small improvements and bug fixes
  
[2.0 WIP6]
* Port of SNES9X 1.50
* SMB support
* SD support
* Greatly improved emulation and timing for NTSC roms
* Save states (freezes) to SD and SMB
* Screen zoom
* Improved font and display
* ROM injector
* ... and more ...


## CREDITS

                      Coding & menu design                           Tantric
                      Additional coding                          michniewski
                      Menu artwork                      NiuuS, the3seashells
                      Menu sound                                Peter de Man
                      Extra coding   Zopenko, Burnt Lasagna, Askot, emukidid
                              NiuuS, Bladeoner, libertyernie, InfiniteBlueGX

                      ¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨¨
                      Snes9x GX GameCube                   SoftDev, crunchy2
                                                             eke-eke, others

                      Snes9x                                     Snes9x Team
                      libogc/devkitPPC                  shagkur & wintermute
                      FreeTypeGX                             Armin Tamzarian


## LINKS

                      SNES9X RX Project Page
                      https://github.com/niuus/Snes9xRX

                      SNES9X Project Page
                      https://github.com/snes9xgit/

                      SNES9X GX Project Page
                      https://github.com/dborth/snes9xgx

                      Wii Homebrew Community
                      https://wiibrew.org/

                      Free (Public Domain) ROMs
                      https://pdroms.de/
					  https://www.retroveteran.com/

                      Cheat Codes
                      www.cheatzilla.com

					  BS-X Project
					  https://project.satellaview.org/
