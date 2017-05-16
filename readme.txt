Theme 'ComicBook' v2.3 - 04-29-2017 by TMNTturtlguy
Theme File Structure based on "carbon" Eric Hettervik (Rookervik) RYOKAI.DEVIANTART.COM
Controller.svg from "carbon" Eric Hettervik (Rookervik) RYOKAI.DEVIANTART.COM
Theme Concept based on images posted by: lipebello on Retropie.org.uk/forum
For use with EmulationStation (http://www.emulationstation.org/)

Special thanks to all who helped:
- modmaster - for helping create additional system backgrounds
- pjft - for all the support throughout the build, testing, and work on the pixel effect
- Nismo - for all of the testing, input, and suggested improvements

This theme is designed for 16:9 aspect ratio only.  It will work on small screens and is tested to work on up to 55" 4K HDTV with excelent quality
-it was noticed on some TV (LG HDTV) that the raspberry Pi picture is zoomed when the TV is set to 16:9.  Change the TV ratio to "list". All other Tv's work 16:9
-To be sure the theme is displayed correctly, there should be a gray border around all sides of the theme.

Theme is designed to be used with the slide transition.

To run this theme smoothly with the slide tranistion. Due to Optimization, there are no issues with performance.  VRAM should be set to 100.

v2 is designed on EmulationStation with maxSize for video and carasoul updates.  It also works on the udpated Screensaver OMX build by @pjft on Apr2017
-Video and images will work properly on both VLC and OMX players. 
-If running on an older of ES without maxSize.  Edit line 78 of comic_book.xml to <size>.
-If running ES with carousel build, the games available should be in comic book font.  If not up to date, standard font will show.

Fonts:
Users can use any font they would like with the theme. Just copy your font to /etc/emulationstation/themes/ComicBook/art folder. 

Gamelist Font Size:
To change the font size of the Gamelist, open the "ComicBook.xml" with a text editor, look for the tag <gamelist> and find a tag inside called <fontSize>. The original value is 0.03. A small change makes a big difference in size. If you want smaller gamelist names, try 0.02. If you want larger, try 0.04. You can even go further by trying 0.015.

Colors:
To change the colors open ComicBook.xml with a text editor. Choose a color and find it's hexidecimal value. Some examples are found in the carbon.xml file. Find all occurances of "8b0000" and replace them with your chosen color. Such as Orange: ef710b. Save the carbon.xml and exit. To change the color to another color after the first change, search for your old color, and replace it with a new one.

Sounds:
- To change the sound effect, replace /art/scroll.wav with what ever WAV file you would like. ComicBook theme will play what ever is called "scroll.wav" in the /art folder.
- Some systems have launching sounds, for example NES plays a coin sound at launch.  To remove the launch sound, edit the theme.xml in the system folder within ComicBook Theme.
- To add launch sound add this to the theme.xml for the system:
		<sound name="launch">
			<path>./../art/XXXX.wav</path>
		</sound>
XXXX = the name of the .wav file.  Add the .wav file to the art forlder.

Game Hacks Sytem views Available:
- add the following to your roms foler and es_systems.cfg. The abbreviation letters should be the name of the rom folder and the name of the theme in the es_system.cfg Simply copy your roms from the regular system into tne roms folder and apply hacks.
- gbh (game boy)
- gbah (game boy advanced)
- nesh (nes)
- snesh (snes)
- ggh (game gear)
- genh (genesis)

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
-Scraped art "md_image" wil be displayed in teh bottom gray box to the right of the video.
-YOU MUST HAVE AT LEAST 1 VIDEO in each systems gamelist in order for this to work.  If you do not have a video for a system YOU MUST:
-If you do not have a video for a system: Open the theme.xml in the systems folder.  Delete lines 53-57 "md_image"  The bottom gray box will be blank, but the scraped art will appear full size in the large black box.
-If you have at least 1 video, the scraped art "md_image" will appear in both the Large Black box and the small gray box for all games that are missing videos.
	 

Systems in Theme:
3D0
amstrad pc
apple 2
Aracde
Atari 2600
atari 5200
Atari 7800
atari lynx
atari st
c64
colecovision
CPS I
CPS II
CPS III
daphne
Dreamcast
Famicom
GB
Game Boy Hacks
GBA
Game Boy Advance Hacks
GBC
game gear
Game Gear Hacks
Game and Watch
Genesis
intellisvion
Kodi
master system
mega drive
msx
N64
NDS
neo geo
NES
ngp
ngpc
NES Hacks
pc engine
ports
PSX
PSP
Retropie (menu)
scummvm
Sega 32X
Sega CD
Sega Genesis Hacks
SG-1000
SNES
SNES Hacks
Super Famicom
Super Grafx
Turbo Grafix 16
vectrex
Virtual Boy
wonderswan
wonderswan color
ZX Spectrum

All other themes are set to work with a generic comic background to match the rest of the theme.  The system logo will be the standard logo from the Carbon Theme.  On the detailed view  They sytem logo will appear twice at the top of the screen.


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
	Added following system logos
		Atari 800
		Atari Jaguar
		AGS
		bbc micro
		Channel f
		coco
		desktop
		dragon 32
		oric
		pce-cd
		residual vm
		saturn
		stratagus
		ti99
		trs80
		videopac
		zmachine
	Completed following Systems
		3D0
		amstrad cpc
		apple 2
		atari St
		c64
		colecovision
		game and watch
		intellivision
		kodi
		MSX
		ports
		vectrex
		Wonderswan Colors
		Wonderswan
		
		
	


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

