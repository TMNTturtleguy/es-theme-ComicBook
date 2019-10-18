Theme 'ComicBook' v2.6 - 06-13-2017 by TMNTturtlguy
Controller.svg from "carbon" Eric Hettervik (Rookervik) RYOKAI.DEVIANTART.COM
Theme Concept based on images posted by: lipebello on Retropie.org.uk/forum
For use with EmulationStation (http://www.emulationstation.org/)

Special thanks to all who helped:
- modmaster - for helping create additional system backgrounds
- holy2tack - for creating several collection themes
- pjft - for all the support throughout the build, testing, and work on the pixel effect
- Nismo - for all of the testing, input, and suggested improvements
- Ruckage - for updating font characters to support multiple languages.

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
- gbh (game boy)
- gbah (game boy advanced)
- nesh (nes)
- snesh (snes)
- ggh (game gear)
- genh (genesis)

Capcom Systems Available (copy your arcade system from es_systems.cfg)
- cps1
- cps2
- cps3

Custom Systems Available
- Adventure Game Studio (ags)
- All Games (auto-allgames)
- Arcade (arcade)
- Batman (batman)
- Beat'em Up (btmups)
- Breath of Fire (breathoffire)
- Capcom (capcom)
- Chrono Trigger (chrono)
- Crash Bandicoot (chrashbandicoot)
- Donkey Kong (donkeykong)
- Favorites (auto-favorites)
- Fighting (fighting)
- Final Fantasy (finalfantasy)
- Fire Emblem (fireemblem)
- Kids (kids)
- Kirby (kirby)
- Kodi (kodi)
- Last Played (auto-lastplayed)
- Legend of Zelda, The (zelda)
- Light Gun (lightgun)
- Mario (mario)
- Mega Man (megaman)
- Metroid (metroid)
- Pokemon (pokemon)
- Ports (ports)
- Racing (racing)
- Retropie Menu (retropie)
- Secret of Mana (secretofmana)
- Shoot'em Up (shmups)
- Sonic (sonic)
- Spyro (spyro)
- Sports (sports)
- Tales of (tales)
- TMNT (tmnt)
- Trackball (trackball)


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
3do
amiga
amstrad pc
apple2
atari800
atari2600
atari5200
atari7800
atarijaguar
atarilynx
atarist
bbc micro
c64
channelf
coco (tandy)
colecovision
daphne
dreamcast
dragon32
famicom
fds
gb
gba
gbc
gamegear
gameandwatch
gc
genesis
intellisvion
macintosh
mastersystem
megadrive
msdos
msx
msx2
n64
nds
neogeo
nes
ngp
ngpc
odyssey2
oric
pcengine
pce-cd
psp
pspminis
psx
ps2
residualvm
saturn
scummvm
sega32x
segacd
sfc
sg-1000
snes
steam
stratagus
supergrafx
turbografix16
turbografixcd
vectrex
videopac
virtualboy
wii
wiiu
wonderswan
wonderswancolor
zxspectrum

All other themes are set to work with a generic comic background to match the rest of the theme.  The system logo will be the standard logo from the Carbon Theme.  On the detailed view the system logo will appear twice at the top of the screen.


Changelog
=========
v2.0 4-18-2017
	Updated to main ES Branch
		implemented <maxSize> on line 78
			<maxSize>0.44 0.42</maxSize>
	Added System Logos for the following systems:
		FB Alpha
		Mame
		Mame-advmame
		Mame-Libretro
		Mame-mame4all
		Mega Drive
		NeoGeo
		Ports
		ScummVM
		Steam
		
v2.1 4-19-2017
	md_image in video/detail view changed to maxSize
	Marquee conflict resolved
		Marquee removed from all systems except actual arcade cabinet systems
		2nd System Logo removed from arcade cabinet systems
		md_marquee deleted from comic_book.xml and moved to theme.xml
	launch sounds added to all sega systems
	comic backgrounds updated for FB Alpha and all Mame systems to match the Arcade background for the time being.
	Comic background updated for all sega systems to match sega genesis background for the time being.
	
v2.2 4-20-2017
	Marquee conflict resolved
		Added marquee back to comic_book.xml and moved off of screen.
	md_image below controller centered.
	
v2.3 4-28-2017
	sega cd border corrected
	all backgrounds optimized to 720 resolution
	removed all unused files from theme folders
	optimized md image on video view to largest max size that will fit in the square area
	Changed system info font to comic style font (will show as normal text in non updated systems)
	Added the following systems:
		atari 5200
		atari lynx
		daphne
		Famicom
		Game Boy Hacks
		Game Boy Advance Hacks
		game gear
		Game Gear Hacks
		master system
		mega drive
		neo geo
		ngp
		ngpc
		NES Hacks
		pc engine
		Sega 32X
		Sega CD
		Sega Genesis Hacks
		SG-1000
		SNES Hacks
		Super Famicom
		Super Grafx
		Turbo Grafix 16
		Virtual Boy
		ZX Spectrum
		
	Added the following system logos:
		3DO
		amstrac cpc
		apple 2
		atari st
		atari lynx
		atari 5200
		c64
		colecovision
		daphne
		famicon 
		fds
		game gear
		game and watch
		intellivision
		kodi
		master system
		macintosh
		msx
		neo geo pocket
		neo geo pocket color
		odyssey2
		pc (ms DOS)
		pc-engine
		sega 32x
		sega CD
		sg-1000
		supergrafx
		super famicom
		turbo graphics 16
		turbo graphics CD
		vectrex
		wonderswan
		wonderswan color
		zx specturm

v2.4 5-
	Feature tags added to comic_book.xml for carousel and video
	Changed the border .SVG to .PNG to optimize the theme.
	Added Comic Rip Mascot
	Corrected Master System System Logo
	Corrected All Turbo Grafx system logos
	changed snes logo to classic purple color scheme
	Optimized the following backgrounds: Arcade, Atari Lynx, gbah, gb, genh, ggh, ngp, snesh 
	Removed the letter a from line one of all theme files.
	corrected the following logos (line of floating pixels removed) lynx, msx, wonderswan, vertex, Oddyssey2, macintosh, apple2, famicom, gbah, atari st, amiga, C64, 3D0, sg-100
	   virtual boy, daphne, Kodi, game and watch, PC Engine, ZX Spectrum, sega 32X, sega cd, mame, fba, ports, neogeo, steam
	Added new Systems:
		cps1
		cps2
		cps3
		capcom
	Completed following Systems
		3D0
		amstrad cpc
		apple 2
		Atari 800
		Atari Jaguar
		atari St
		AGS
		bbc micro
		c64
		Channel f
		colecovision
		coco
		desktop
		dragon 32
		game and watch
		intellivision
		kodi
		MSX
		oric
		pce-cd
		ports
		residual vm
		saturn
		stratagus
		ti99
		trs80
		videopac
		vectrex
		Wonderswan Colors
		Wonderswan
		zmachine

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


License
=======

-------------------------------------------------------------------------

Summary of the license below:

ALLOWED:      - Share and duplicate as it is
              - Edit, alter, change it

REQUIREMENTS: - Attribution, give credit to the creator
              - Indicate changes to it
              - Publish the changes under the same license

PROHIBITED:   - Commercial distribution

-------------------------------------------------------------------------

LOGO NOTICE

The used logos and trademarks are copyright of their respective owners.

-------------------------------------------------------------------------

