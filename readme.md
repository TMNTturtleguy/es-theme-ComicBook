# Theme 'ComicBook'
![Preview 1](https://raw.githubusercontent.com/Zenjir0/es-theme-ComicBook/3.2-Beta/_assets/previews/Preview%201.png)

![Preview2](https://raw.githubusercontent.com/Zenjir0/es-theme-ComicBook/3.2-Beta/_assets/previews/Preview%202.png)

Update 3.2 - 04-21-2020 by [Zenjiro](https://retropie.org.uk/forum/user/zenjiro)\
Theme Concept based on images posted by: [lipebello](https://retropie.org.uk/forum/user/lipebello) on Retropie.org.uk/forum\
For use with [EmulationStation](https://emulationstation.org/index.html)

## Recommended EmulationStation Forks:
* [EmulationStation FCAMOD](https://github.com/fabricecaruso/EmulationStation/releases) by [fabricecaruso](https://retropie.org.uk/forum/user/f-caruso) - Optimized for Windows
* [RetroPie EmulationStation](https://github.com/jrassa/EmulationStation/releases) by [jrassa](https://retropie.org.uk/forum/user/jdrassa) - Retropie EmulationStation ported to Windows


## Special Thanks to all who helped:
- [TMNTturtlguy](https://retropie.org.uk/forum/user/tmntturtlguy) - for creating such an iconic theme
- [modmaster](https://retropie.org.uk/forum/user/modmaster)    - for helping create additional system backgrounds
- [holy2tack](https://retropie.org.uk/forum/user/holy2tack)    - for creating several collection themes
- [pjft](https://retropie.org.uk/forum/user/pjft)         - for all the support throughout the build, testing, and work on the pixel effect
- [Nismo](https://retropie.org.uk/forum/user/nismo)        - for all of the testing, input, and suggested improvements
- [Ruckage](https://retropie.org.uk/forum/user/ruckage)      - for updating font characters to support multiple languages.
- Safemode     - for testing debuging, and critque help
- Elcie 	   - for Image editing and insight help

## Important Information

This theme is designed for **16:9 aspect ratio only!!!**

This is a **HARD FORK** of [TMNTturtlguy's](https://retropie.org.uk/forum/user/tmntturtlguy) theme. Meaning you should do a clean install of this version, and not just copy over your old version. If you do expect issues. Several underlying aspects have been changed.

Thanks to new optimization and ES updates by [pjft](https://retropie.org.uk/forum/user/pjft) there are no issues with performance.  VRAM should be set to 100.

See UserModInstruct.txt for instructions on available user modifications.

## Installation

## TODO

## History??

2.0 is designed on EmulationStation with maxSize for video and carousel updates.  It also works on the updated Screensaver OMX build by [pjft](https://retropie.org.uk/forum/user/pjft) on Apr2017
-Video and images will work properly on both VLC and OMX players.
-If running on an older of ES without maxSize.  Edit line 78 of comic_book.xml to `<size>`.
-If running ES with carousel build, the games available should be in comic book font.  If not up to date, standard font will show.

Example for es_systems.cfg - copied gba and modified `<name>`, `<path>`, `<platform>`, and `<theme>` to gbah

  ```
  <system>
    <name>gbah</name>
    <fullname>Game Boy Advance Hacks</fullname>
    <path>/home/pi/RetroPie/roms/gbah</path>
    <extension>.7z .gba .zip .7Z .GBA .ZIP</extension>
    <command>/opt/retropie/supplementary/runcommand/runcommand.sh 0 _SYS_ gba %ROM%</command>
    <platform>gbah</platform>
    <theme>gbah</theme>
  </system>
  ```

The theme is designed for use with video preview.
- The detail (Video View) will play the preview video "md_video" in the large black box.
- Scraped art "md_image" will be displayed in the bottom gray box to the right of the video.
- If you have at least 1 video, the scraped art "md_image" will appear in both the Large Black box and the small gray box for all games that are missing videos.

The theme is optimized for 2D Box Art and Screenshots - 3D boxart will work, however it may not fill the designated area.

All other themes are set to work with a generic comic background to match the rest of the theme.  The system logo will be the standard logo from the Carbon Theme.  On the detailed view the system logo will appear twice at the top of the screen.


## Changelog
---
### Version 2.0 -> v2.6 
- Changes can be found in parent repository https://github.com/TMNTturtleguy/es-theme-ComicBook

### Version 3.0
NOTE: Consider this a HARD fork of TMNTturtleguy's 16:9 version of ComicBook Theme.\
	Over 2 years and still one of the best looking themes.\
	This is a fork of TMNTturtleguy's 16:9 version of ComicBook Theme. I do not plan on doing anything with the 4:3 variant.\
	HIGHLY RECOMMEND: That you do NOT overwrite your old 'comicbook' theme folder with this one.
	Many of the files and directories have changed or been relocated.\
	Biggest change is to the directory structure. There is no longer an 'art' folder in each of the theme's directory.\
	The reasoning behind this change is to make it as simple as possible for anyone to create/submit a new theme.\
	All one has to do is create a folder and placing a few key files in it.\
	All you need, is to place your own comic and system.png files in the folder, and copy the theme.xml from the 'template' theme folder.\
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

### Version 3.1

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

### Version 3.2
	Upscaled older system image files by a factor of 2 using Waifu2x.
	Removed Tutorial archive
	Removed Unused assets
	Optimized all PNG images to 128-bit color using PNGquant
	Moved launch WAV files to corresponding "hacks" systems
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

## Collection Rework Status
|*System*|*System Image*|*Banner Logo*|*Comic*|*Comic Rip*|*Launch Sound*|
|--------|--------------|-------------|-------|-----------|--------------|
|Test|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|:heavy_check_mark:|