Theme 'ComicBook' by TMNTturtlguy
Update 3.1 - 12-16-2019 by Zenjiro
Controller.svg from "carbon" Eric Hettervik (Rookervik) RYOKAI.DEVIANTART.COM
Theme Concept based on images posted by: lipebello on Retropie.org.uk/forum
For use with EmulationStation (http://www.emulationstation.org/)

Recommended EmulationStation Forks:
fabricecaruso (https://github.com/fabricecaruso/EmulationStation/releases)
jrassa        (https://github.com/jrassa/EmulationStation/releases)

Special thanks to all who helped:
- modmaster - for helping create additional system backgrounds
- holy2tack - for creating several collection themes
- pjft      - for all the support throughout the build, testing, and work on the pixel effect
- Nismo     - for all of the testing, input, and suggested improvements
- Ruckage   - for updating font characters to support multiple languages.
- Safemode  - for testing and debuging help
- Elcie 	- for GIMP and Image editing help

This theme is designed for 16:9 aspect ratio only.  It will work on small screens and is tested to work on up to 55" 4K HDTV with excellent quality
-it was noticed on some TV (LG HDTV) that the raspberry Pi picture is zoomed when the TV is set to 16:9.  Change the TV ratio to "list". All other TV's work 16:9
-To be sure the theme is displayed correctly, there should be a gray border around all sides of the theme.

Thanks to new optimization and ES updates by @pjft there are no issues with performance.  VRAM should be set to 100.

See UserModInstruct.txt for instructions on available user modifications.

v2 is designed on EmulationStation with maxSize for video and carousel updates.  It also works on the updated Screensaver OMX build by @pjft on Apr2017
-Video and images will work properly on both VLC and OMX players.
-If running on an older of ES without maxSize.  Edit line 78 of comic_book.xml to <size>.
-If running ES with carousel build, the games available should be in comic book font.  If not up to date, standard font will show.

Game Hacks System views Available:
- add the following to your roms folder and es_systems.cfg. The abbreviation letters should be the name of the rom folder and the name of the theme in the es_system.cfg Simply copy your roms from the regular system into the roms folder and apply hacks.
- gbh   (game boy)
- gbah  (game boy advanced)
- nesh  (nes)
- snesh (snes)
- ggh   (game gear)
- genh  (genesis)

Capcom Systems Available (copy your arcade system from es_systems.cfg)
- cps1
- cps2
- cps3

Custom Systems Available
- Adventure Game Studio (ags)
- All Games             (auto-allgames)
- Arcade                (arcade)
- Batman                (batman)
- Beat'em Up            (btmups)
- Breath of Fire        (breathoffire)
- Capcom                (capcom)
- Chrono Trigger        (chrono)
- Crash Bandicoot       (chrashbandicoot)
- Donkey Kong           (donkeykong)
- Favorites             (auto-favorites)
- Fighting              (fighting)
- Final Fantasy         (finalfantasy)
- Fire Emblem           (fireemblem)
- Kids                  (kids)
- Kirby                 (kirby)
- Kodi                  (kodi)
- Last Played           (auto-lastplayed)
- Legend of Heroes, The (legendofheroes)
- Legend of Zelda, The  (zelda)
- Light Gun             (lightgun)
- Mario                 (mario)
- Mega Man              (megaman)
- Metroid               (metroid)
- Pokemon               (pokemon)
- Ports                 (ports)
- Racing                (racing)
- Retropie Menu         (retropie)
- Secret of Mana        (secretofmana)
- Shoot'em Up           (shmups)
- Sonic                 (sonic)
- Spyro                 (spyro)
- Sports                (sports)
- Tactic Ogre           (tacticogre)
- Tales of              (tales)
- TMNT                  (tmnt)
- Trackball             (trackball)


Example for es_systems.cfg - copied gba and modified <name>, <path>, <platform>, and <theme> to gbah
<system>
    <name>gbah</name>
    <fullname>Game Boy Advance Hacks</fullname>
    <path>/home/pi/RetroPie/roms/gbah</path>
    <extension>.7z .gba .zip .7Z .GBA .ZIP</extension>
    <command>/opt/retropie/supplementary/runcommand/runcommand.sh 0 _SYS_ gba %ROM%</command>
    <platform>gbah</platform>
    <theme>gbah</theme>
  </system>

The theme is designed for use with video preview.
-The detail (Video View) will play the preview video "md_video" in the large black box.
-Scraped art "md_image" will be displayed in the bottom gray box to the right of the video.
-If you have at least 1 video, the scraped art "md_image" will appear in both the Large Black box and the small gray box for all games that are missing videos.

The theme is optimized for 2D Box Art and Screenshots - 3D boxart will work, however it may not fill the designated area.


Systems in Theme:
3DO                  (3do)
Amiga                (amiga)
Amiga CD             (amigacd32)
Amstrad CPC          (amstradcpc)
Apple 2              (apple2)
Atari 800            (atari800)
Atari 2600           (atari2600)
Atari 5200           (atari5200)
Atari 7800           (atari7800)
Atari Jaguar         (atarijaguar)
Atari Lynx           (atarilynx)
Atari ST             (atarist)
BBC Micro            (bbcmicro)
Commodore 64         (c64)
Channel F            (channelf)
Tandy Color Computer (coco)
Colecovision         (colecovision)
Daphne Emulator      (daphne)
Dreamcast            (dreamcast)
dragon32             (dragon32)
Famicom              (famicom)
Famicom Disk System  (fds)
Game Boy             (gb)
Game Boy Advance     (gba)
Game Boy Color       (gbc)
Game Gear            (gamegear)
Game & Watch         (gameandwatch)
GameCube             (gc)
Genesis              (genesis)
Intellisvion         (intellisvion)
Macintosh            (macintosh)
Mastersystem         (mastersystem)
Mega Drive           (megadrive)
MS-DOS               (msdos)
MSX                  (msx)
MSX2                 (msx2)
Nintendo 64          (n64)
Nintendo DS          (nds)
Neo Geo              (neogeo)
NES                  (nes)
Neo Geo Pocket       (ngp)
Neo Geo Pocket Color (ngpc)
Odyssey 2            (odyssey2)
Oric                 (oric)
PC Engine            (pcengine)
PC Engine CD         (pce-cd)
PlayStation Portable (psp)
PSP Minis            (pspminis)
PlayStation          (psx)
PlayStation 2        (ps2)
ResidualVM           (residualvm)
Saturn               (saturn)
ScummCM              (scummvm)
Sega 32X             (sega32x)
Sega CD              (segacd)
Super Famicom        (sfc)
SG-1000              (sg-1000)
SNES                 (snes)
Steam                (steam)
Stratagus            (stratagus)
SuperGrafx           (supergrafx)
TurboGrafix-16       (turbografix16)
TurboGrafix-CD       (turbografixcd)
Vectrex              (vectrex)
Videopac             (videopac)
Virtual Boy          (virtualboy)
Wii                  (wii)
Wii U                (wiiu)
WonderSwan           (wonderswan)
WonderSwan Color     (wonderswancolor)
ZX Spectrum          (zxspectrum)

All other themes are set to work with a generic comic background to match the rest of the theme.  The system logo will be the standard logo from the Carbon Theme.  On the detailed view the system logo will appear twice at the top of the screen.


Changelog
=========
v2.0	4-18-2017
	Updated to main ES Branch
		implemented <maxSize> on line 78
			<maxSize>0.44 0.42</maxSize>
	Added System Logos for the following systems:
	- FB Alpha
	- Mame
	- Mame-advmame
	- Mame-Libretro
	- Mame-mame4all
	- Mega Drive
	- NeoGeo
	- Ports
	- ScummVM
	- Steam

v2.1	4-19-2017
	md_image in video/detail view changed to maxSize
	Marquee conflict resolved
		Marquee removed from all systems except actual arcade cabinet systems
		2nd System Logo removed from arcade cabinet systems
		md_marquee deleted from comic_book.xml and moved to theme.xml
	Launch sounds added to all sega systems
	Comic backgrounds updated for FB Alpha and all Mame systems to match the Arcade background for the time being.
	Comic background updated for all sega systems to match sega genesis background for the time being.

v2.2	4-20-2017
	Marquee conflict resolved
		Added marquee back to comic_book.xml and moved off of screen.
	md_image below controller centered.

v2.3	4-28-2017
	Sega CD border corrected
	All backgrounds optimized to 720 resolution
	Removed all unused files from theme folders
	Optimized md image on video view to largest max size that will fit in the square area
	Changed system info font to comic style font (will show as normal text in non updated systems)

	Added the following systems:
	- atari 5200
	- atari lynx
	- daphne
	- Famicom
	- Game Boy Hacks
	- Game Boy Advance Hacks
	- game gear
	- Game Gear Hacks
	- master system
	- mega drive
	- neo geo
	- ngp
	- ngpc
	- NES Hacks
	- pc engine
	- Sega 32X
	- Sega CD
	- Sega Genesis Hacks
	- SG-1000
	- SNES Hacks
	- Super Famicom
	- Super Grafx
	- Turbo Grafix 16
	- Virtual Boy
	- ZX Spectrum

	Added the following system logos:
	- 3DO
	- amstrac cpc
	- apple 2
	- atari st
	- atari lynx
	- atari 5200
	- c64
	- colecovision
	- daphne
	- famicom
	- fds
	- game gear
	- game and watch
	- intellivision
	- kodi
	- master system
	- macintosh
	- msx
	- neo geo pocket
	- neo geo pocket color
	- odyssey2
	- pc (ms DOS)
	- pc-engine
	- sega 32x
	- sega CD
	- sg-1000
	- supergrafx
	- super famicom
	- turbo graphics 16
	- turbo graphics CD
	- vectrex
	- wonderswan
	- wonderswan color
	- zx specturm

v2.4	5-
	Feature tags added to comic_book.xml for carousel and video
	Changed the border .SVG to .PNG to optimize the theme.
	Added Comic Rip Mascot
	Corrected Master System System Logo
	Corrected All Turbo Grafx system logos
	Changed snes logo to classic purple color scheme
	Optimized the following backgrounds: Arcade, Atari Lynx, gbah, gb, genh, ggh, ngp, snesh
	Removed the letter a from line one of all theme files.

	Corrected the following logos (line of floating pixels removed):
	lynx, msx, wonderswan, vertex, Oddyssey2, macintosh, apple2, famicom, gbah, atari st, amiga, C64, 3D0, sg-100,
	virtual boy, daphne, Kodi, game and watch, PC Engine, ZX Spectrum, sega 32X, sega cd, mame, fba, ports, neogeo, steam

	Added new Systems:
	- cps1
	- cps2
	- cps3
	- capcom

	Completed following Systems
	- 3D0
	- amstrad cpc
	- apple 2
	- Atari 800
	- Atari Jaguar
	- atari St
	- AGS
	- bbc micro
	- c64
	- Channel f
	- colecovision
	- coco
	- desktop
	- dragon 32
	- game and watch
	- intellivision
	- kodi
	- MSX
	- oric
	- pce-cd
	- ports
	- residual vm
	- saturn
	- stratagus
	- ti99
	- trs80
	- videopac
	- vectrex
	- Wonderswan Colors
	- Wonderswan
	- zmachine

v2.5	5-21-17
	Modified detailed view so image will show in black box properly.
	updated github so that extra files have been removed from download.

v2.6	6-13-17
	Changed Comic Rip for Sega CD and Sega 32X
	Corrected Channel F controller in system background
	Renamed trs80 to trs-80 to match es_systems.cfg
	Updated font to allow special characters for different languages - Thank you to Ruckage for supplying the font!
	Updated size of video and image in black box
	Updated to better support detailed view
	Update for colors support for ratings

	Added the following Themes:
	- All Games
	- Batman
	- Beat'em Up
	- Favorites
	- Fighting
	- Gamecube
	- Kids
	- Last Played
	- Light Gun
	- Mario
	- Mega Man
	- MSX2
	- PS2
	- PSP Minis
	- Racing
	- Shoot'em Up
	- Sonic
	- Sports
	- TMNT
	- Trackball
	- Wii
	- WiiU

v3.0  	11-11-19
	NOTE: Consider this a HARD fork of TMNTturtleguy's 16:9 version of ComicBook Theme.
	Over 2 years and still one of the best looking themes.
	This is a fork of TMNTturtleguy's 16:9 version of ComicBook Theme. I do not plan on doing anything with the 4:3 variant.
	HIGHLY RECOMMEND: That you do NOT overwrite your old 'comicbook' theme folder with this one.
	Many of the files and directories have changed or been relocated.
	Biggest change is to the directory structure. There is no longer an 'art' folder in each of the theme's directory.
	The reasoning behind this change is to make it as simple as possible for anyone to create/submit a new theme.
	All one has to do is create a folder and placing a few key files in it.
	All you need, is to place your own comic and system.png files in the folder, and copy the theme.xml from the 'template' theme folder.
	You can also add a comic_rip.png, and launch.wav in the same folder to make a dynamic and immersive experience.

	Changed the following:
	- Simplified directory structure. All contents in the 'art' folder in each theme have been moved to the parent's folder.
	- The 'art' folder was renamed to '_assets'
	- Theme 'TMNT' was renamed to 'tmnt'
	- Renamed all 'system 3' image files to 'bannerlogo'
	- All 'rip' images were renamed to 'comic_rip'
	- All 'comic_rip' images were moved to their respective theme folders
	- All 'launch' sound files were moved to their respective theme folders and renamed to 'launch.wav'
	- Removed 'misc' theme, 'Template' replaces this theme
	- Removed 'love' theme, 'Favorites' replaces this theme
	- Removed 'tg16cd' theme, it was identical to 'tg-cd'theme
	- Many aracde themes such as, 'arcade', 'mame', 'mame4all', etc had their bannerlogo turned on. It was previously off.
	- Renamed 'coco' theme to 'tandy'

	Added the following:
	- The 'template' theme
	- This theme folder contains a blank theme. It was created as a guide for those who wish to create new collection or system themes.
	- There is also a 7z archive containing tutorials on how to create certain images and assets for this project.
	- All comic_rip images, launch sound files, etc where added and properly named in the '_assets' folder.
	- Added TMNTturtleguy's Adobe Photoshop .psd and .ai template files to the '_assets' folder.


	Updated the following:
	- The 'batman' theme now has a 'Batman Spinning Logo' launch sound, and the 'bannerlogo' has been updated.
	- The 'starwars' theme now has a 'Light-Saber Activation' launch sound
	- The 'sonic' theme now has a 'Sonic Got an Emerald' launch sound
	- The 'tmnt' theme now has a 'Cowabunga!' launch sound

	Added the following Themes by Holy2tack:
	- Breath of Fire
	- Chrono Trigger
	- Crash Bandicoot
	- Donkey Kong
	- Final Fantasy
	- Fire Emblem
	- Kirby
	- Legend of Heroes, The
	- Legend of Zelda, The
	- Metroid
	- Pokemon
	- Secret of Mana (Seiken Densetsu)
	- Spyro
	- Tactics Ogre
	- Tales of Series

	Added Themes:
	- Banjo Kazooie

	Work-in-Progress
	- More Themes to Come
	- Upscale older images for Raspberry Pi 4 and Windows Machines

v3.1  	12-16-19
	Optimized several PNG files bringing the repo zip file size down to 143MB from 243MB
	Converted all newer 1080p comic PNG files to 720p. This fixes loading issues on the Raspberry Pi

	Updated the following:
	- MESS theme now has a proper system image
	- SamCoup'e now has a proper system image

	Added Systems:
	- FB Neo
	- PS3
	- Xbox
	- Xbox 360

	Added Themes:
	- Bomberman
	- Castlevania
	- Disney
	- Luigi
	- Mass Effect
	- Mega Man Classic
	- Mega Man X
	- Mega Man Zero
	- Simpsons
	- Tomb Raider

v3.2  00-00-20
	Upscaled older system image files by a factor of 2 using Waifu2x.
	Removed Tutorial archive
	Removed unused assets
	Optimized all PNG images to 128-bit color using PNGquant
	Moved launch WAV files to corrisponding "hacks" systems
	Replaced all SVG files with PNG files
	Removed all "controller" images

	Fixed the Following:
	- Renamed chrashbandicoot to crashbandicoot

	Changed the Following:
	- PC is now MSDOS

	Added Systems:
	- Atomiswave
	- Auto-at2players
	- Auto-at4players
	- Auto-neverplayed
	- C64-Classic
	- Capcom-Classic
	- Famicom-Classic
	- Famicom-Shonen
	- Mega CD
	- Mega Drive-Japan
	- Naomi
	- Neo-Geo CD
	- NES-Classic
	- Nintendo 3DS
	- Nintendo 64DD
	- PC
	- PC-88
	- PC-98
	- PlayStation-Classic
	- Pokemon Mini
	- Satellaview
	- SFC-Classic
	- SNES-Classic-US
	- SNES-Classic-EU
	- Sufami Turbo
	- Nintendo Switch
	- Sharp X1
	- Sharp X68000

	Added Themes:
	- Advance Wars
	- Animal Crossing
	- Ape Escape
	- Blizzard
	- Custom Robo
	- Darkstalkers
	- Diablo
	- Doom
	- Dot Hack
	- Dragon Quest
	- Earthbound
	- Golden Sun
	- Halo
	- Humongous Entertainment
	- JRPG
	- Kingdom Hearts
	- Konami
	- Metal Gear
	- Mother
	- Pac-man
	- Phantasy Star
	- Pheonix Wright
	- Ratchet & Clank
	- Rayman
	- Shining Force
	- Starcraft
	- Starfox
	- Star Ocean
	- Star Trek
	- Street Fighter
	- Warcraft
	- Wario
	- Witcher
	- Yoshi