# Miyoo Mini+
This is a write-up explaining the Miyoo Mini+ and how to set it up.
<img src=https://retrododo.com/wp-content/uploads/2023/03/miyoo-mini-plus-pokemon-1160x653.webp>
## About
The Miyoo Mini+ is one of several new handheld emulators that have been released. An emulator is a piece of software that acts like it is a piece of hardware, like a game console, and then it is able to read "ROMs" like they are being read on the original hardware.
- Audio
  - 3.5mm Headphone jack
  - Speaker
  - Bluetooth
- Wifi
  - Update achievements online
  - Play local multiplayer games like they are wireless
  - Play multiplayer games over the wifi
  - Sync roms remotely over SSH/FTP
- Smaller than a phone, larger screen than a Gameboy 

## Hardware
- [Miyoo Mini+](https://www.amazon.com/Miyoo-Mini-Plus-Handheld-Dedicated/dp/B0CB6TQ3H1/ref=sr_1_5?crid=2VQRWKHEE57G3&keywords=miyoo+mini+plus&qid=1694445184&sprefix=miyoo%2Caps%2C199&sr=8-5&ufe=app_do%3Aamzn1.fos.18ed3cb5-28d5-4975-8bc7-93deae8f9840) (Comes with case. Screen is fragile. Should be less than $80.)
- [SD Card](https://www.amazon.com/SAMSUNG-microSDXC-Expanded-MB-ME128KA-AM/dp/B09B1JFY24/ref=pd_bxgy_sccl_1/145-7827923-7958051?pd_rd_w=xqmyJ&content-id=amzn1.sym.26a5c67f-1a30-486b-bb90-b523ad38d5a0&pf_rd_p=26a5c67f-1a30-486b-bb90-b523ad38d5a0&pf_rd_r=7TXZQ0NA0TZT932RE302&pd_rd_wg=skWfP&pd_rd_r=e3281e84-0ae3-4088-8403-98dac932d920&pd_rd_i=B09B1JFY24&th=1) (Must buy a new SD card as the default is corruptable.)

## Software
The default software that ships with the Miyoo Mini+ comes with some ROMs and a basic OS. It is strongly advised to install OnionOS on a new SD card and then secure new ROMS. The ones it ships with are not good, and the SD card will fail. The games you will likely want to get achievements in. If you care about that, you will need to make sure to have the same version supported on RetroAchievements, otherwise the version does not matter.
- [OnionOS](https://github.com/OnionUI/Onion/wiki/Installation#download-the-installation-files)
<img src=https://retrogamecorps.files.wordpress.com/2022/01/onion-720p.png>

#### OnionOS Installation Guide
The Miyoo Mini and the Mini+ use different versions at the time of writing this. The link above goes to the Installation instructions from OnionOS. At the time I wrote this, they were on version 4.2.0 release candidate for the Mini+. The regular Mini (not hotlinked above) has different firmware version you must check in the settings first. The instructions for installation are pretty straightforward in that link. 

#### OnionOS Basic Operations
- Refresh ROMs in the games list to see newly added ROMs
- Wifi does not save more than one router at a time, so must manually change when traveling in Settings.
- Menu button to quick switch games
- Menu button then Select to enter the RetroArch screen in game
- Menu button then Start to exit to the OnionOS screen
- In RetroArch settings you can reassign LR buttons
- RetroArch settings to set RetroAchievements profile

## Achievements
If you are interested in tracking your achievements for the old games you are playing, you can sign up for an account at RetroAchievements and then insert those credentials into OnionOS. To unlock the achievement, you must be actively connected to the Internet. (The Miyoo Mini+ has wifi, but cannot remember multiple networks, just a reminder when changing networks.)
-[RetroAchievements](https://retroachievements.org/) 
-[My Profile](https://retroachievements.org/user/Lahey)

<img src=https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjCLV8vMZGRB_ctudvGIYD95Mh-EL9QI4K0Y386t8GCeBCoDs2KCcOouF4nIhHJ2j5okUfnTW9tluFRg3XXNi7oRElf-5CFKNAi7CKrmWk0adSSvaHe62F99S0WC12JxQBbxIbuimED1NtbLTvmLGQ7XJJzefLjc56Ka9He7m_ZyDQV-1ne3so/s1273/retroach.png>

#### Achievement Compatibility
To check and see which ROM is supported on RetroAchievements, go to the game you are interested to play on RetroAchievements and scroll down 75% through the page till you see Supported Game Files. In there, it will have a version number and a hash. You should try to source that same version number. To ensure that you have the correct file after you download, you can compare the hash against the one on the website. The hash on RetroAchievements is the long string of characters under the name of the game file. 

On Windows, you can generate an MD5 hash for the file you downloaded
- Windows + r
- Type `cmd` without quotes then hit enter to open a Command Prompt
- Navigate to the same directory you downloaded the files. If you downloaded to Downloads, then `cd Downloads`.
- `certutil -hashfile <file> MD5`
- EX: `certutil -hashfile "Pokemon Red v1.0.gb" MD5`

#### Hardcore Achievements vs Softcore Achievements
RetroAchievements distinguishes between "hardcore" and "softcore" achievements. The hardcore achievements are achievements that are achieved during hardcore mode. Hardcore mode can be activated in the settings of RetroArch. Hardcore mode disables save states and cheats and other emulator hacks that could make it easier to achieve the achievement than on regular hardware. Softcore achievements are achievements that are unlocked while hardcore mode is not engaged. These mean that the use of emulator tricks could have aided in unlocking the achievement. Some games rely on save states to fullfill saving functionality in the game. These games you will have to beat in one sitting if you want to play in hardcore mode. Most hardcore mode games just set you back to the title screen everytime you play, softcore mode leaves you in the game where you last left off. 

## Games
The Miyoo Mini+ is capable of emulating a wide range of games. Updates to the individual emulators and OnionOS can impact which games are playable, so it is best to search elsewhere. It is safe to assume you can play any NES/SNES/GB/GBC/GBA/PS1/Mega Drive/Genesis game. Some other games for other consoles work as well. 

#### Acquiring ROMs
I am fairly certain it is illegal to directly point you to where to download ROMs, but most ROMs are considered to be abandonware, so they are fairly available. Googling the game you want and ROM should lead you to a myriad of websites. Many ROMs are featured in the Internet Archive, and likewise, there is a Lair owned by a guy whose name is a text editor for Linux that has a good selection of games available. Download these games and sync them to their appropriate directories inside the ROMs directory. FC=Famicom=NES, SFC=Super Famicom=Super Nintendo

#### ROM Hacks
There is a wild world out there these days. For decades, people have been hacking ROMs. But recently, people have gotten really good at working with the decompiled assets of games of the past. The genius programmers of the world are taking assets from existing games and are using them to improve existing games, removing bugs and adding in Quality of Life additions. Some people are even creating entire new games using existing assetts, like a Pokemon game where you play as Team Rocket against the anime's protagonist. Many of these ROM hacks are available to be tracked on RetroAchievements as well. 
