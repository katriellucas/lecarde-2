## Description
Source code of the fan-game Castlevania: The Lecarde Chronicles 2 made by Migami Games. Due to a HDD failure, the original source have been lost. This repo is an atempt to preserve, fix and improve this game.

Unfortunately, the recovery process ended up corrupting all non-English characters, many transparency effects and more. So, if you know any of the following languages and is interested in helping us out by fixing and re-translating this project, feel free to contact us, we are in need of:
- Someone who're both good at Clickteam Fusion 2.5 and good French speakers (preferably)
- Someone who're good at Clickteam Fusion 2.5


## Disclaimer
We contacted Migami Games and got approval to keep this repository up.  

The release of Lecarde Chronicles 2 got permitted by Konami, the game and its assets are freeware and **_SHOULD NOT_** be sold, this also includes the source code. Any modifications you do have also to be free. Castlevania is an intellectual property owned by Konami, please support the company by buying their official releases. 


## Usage
To get the reworked game builds, go to "Releases", choose the latest "v*. *. *-alpha" tag and find the .exe files in the "Game Binary" zipped file. The .exe file is the generated executable, while the .mfa file in "Source Code" zipped file fis the (recovered) Clickteam Fusion project file necessary to generate the .exe (note in this game's case, it requires some extensions from Clickteam Fusion 2.5 Developer builds to be opened). 

Note that the original game is infamous for the compatibility issue for PS4/Xbox controllers if your computers are unlucky so it left the controller preference blank. Here's a valid workaround to this issue if you encountered it like us:

In Control Panel→ Devices and printers, find PS4 controller (usually labeled as "Wireless Controller"), right click "Wireless Controller" label to find controller setting, then click "advance..." to go into advance setting of "Wireless Controller", and be sure the "Wireless Controller" is checked as the preference.

The same could be applied to Xbox Controllers by repeating the setup above while your desired Xbox controller is plugged in.


#### About "LC2_KeyBinding.ini" #### 

A reworked version of the keyboard control created by DragonX24.
This file must be placed in the same directory the game locates if you downloaded the game and moved the game files to a fresh new location.

#### NEW Hotkey Functions #### 

Due to the limitation of original GUI, there're instructions to some new functions that cannot be directly embedded in the GUI...
- Toggle anti-alias on/off: F5/F6

To make the game display 1:1 pixel perfect scale:
- You must make sure the display monitor's vertical size is above 1000.
- You must make sure the windows display scale is exact 100%.
- Toggle anti-alias to off after opening the game.

#### About "Alternate build method" #### 

"Alternate build method" is done as an attempt to keep a small quirk away - when saving at save spots, the game will get stuck for several seconds before finally active again.
This way the game's pack method will be identical to vanilla but will cause antivirus flag to go mad so not recommended unless you want to go with loyalty and purity to vanilla.


#### Read this if antivirus softwares flagged the game as Malware ####
It's something about Clickteam's engine itself. Antivirus softwares don't seem to be too kind towards some Games used Clickteam's engine. If the problem that the antivirus softwares flagged the game as malware occurs, either turn off the antivirus software in question, or add the game to its white list. Also avoid directly sharing the zips or folder(s) which contain the exe file unless really necessary because some net drive safety calculation like Google's, don't seem to be too happy with the game. 

#### Read this if your screen capture program did not work in Reworked LC2 ####
Some capture programs will have compatibility issue with reworked LC2 on Windows 10 (for example, Ocam). This is because the compatibility issue of some revisions of Windows 10's Direct X9 mode. If you want safe screen recording methods, more mainstream programs (like OBS) will work.


#### Read this if you encountered framerate problem in fullscreen mode #### 
It's something about your setting of VSync under Direct X 9 mode. If your only graphic device is a Nvidia GTX graphic card, toggle VSync in your Nvidia control panel to "fast" or "on" if you encountered frame rate problem in fullscreen mode.

#### Known bugs #### 
- If the game's project file is loaded through frame editor, quickly unfocus the game window by overlapping it with a larger window upon proceeding a frame change, when the next frame about to be loaded, the cursor will automatically move upwards. We tried multiple ways but cannot proceed bright results to rule out it. This shouldn't get in the way of normal gameplay on the generated .exes, though.

- If quickly unfocus the game window when holding a direction key at title menu, then focus back, the game's direction input will stuck. This is because the reworked game requires Control X plugin to sufficiently apply newly assigned Keyboard key input dynamically (in DragonX24's remodeled key assign formula) with the structure of such plugin is unfortunately too old and can generate issues with LC2 structure. Shouldn't get in the way of normal gameplay though.


## Changelog

#### [1.4.5] - 2024/3/22 #### 

`ADDED` - Alternate build method of game binary and Infos for alternate build method at readme.  (Aceearly1993)  
`FIXED` - A irregular behavior that sound effects will get overlap when healing at the save point statue under negative status. (Aceearly1993)  
`FIXED` - An oversight that one text size will exceed length of text box in guide section in German language. (Aceearly1993)  


#### [1.4.4] - 2024/3/16 #### 

`CHANGED` - Terminate dx11 text size problems once and for all without breaking the vanilla dx9 text formula. (Aceearly1993)   
`ADDED` - Instructions to make the game run in 1:1 pixel perfect mode.  (Aceearly1993)   
`FIXED` - A irregular behavior that Attack motion will pull out after choosing a destination of ferryman/Garden of the Dead entrance statue.  (Aceearly1993)   
`FIXED` - Hunter skeleton's HP information in enemy bestiary which was wrong in vanilla.  (Aceearly1993)   
`FIXED` - Red glowing effect in Alucard reinforce animation which only had one direction in vanilla.  (Aceearly1993)   


#### [1.4.3] - 2024/3/12 #### 
(Catoblepas)  
`ADDED` - Port the Gorgon 1.4.2 changes on Air Dash (Github issue #43) to Catoblepas build (1.4.0). (Aceearly1993)  

(Gorgon)  
`ADDED` - Translations to enemy description:  
English/Portuguese/Simplified Chinese - The Lecarde 2 rework project team (Aceearly1993, Katriel, ThePlotTwist, Jeffrey Montoya)    
French - Chernabogue   
Spanish - Jorge Fuentes   
German - Exorion Hagen   
Italian - TheCarsEdge   
Japanese - 狼王之2型   
`ADDED` - "S" and "T" labels on save spots and warp spots in oder to let color weak/color blind people 
easier to recognize the location of save spots and warp spots on mini map. (Aceearly1993)    
`ADDED` - Important UIs on start screen to make players not get lost quickly.  (Aceearly1993)    
`ADDED` - A hotkey set so that the game's anti-alias can be toggled on/off to fit the preference of more people.  (Aceearly1993)    
`CHANGED` - In-game credit text to match up the translation contributor lists of Reworked edition.  (Aceearly1993)    
`CHANGED` - Position of text objects in sub screen that got missed for some reason.  (Aceearly1993)    
`FIXED` - Now the game window's position will be automatically re-centered once a window size is chosen in video option screen. (Aceearly1993)     
`FIXED` - A phenomenon that causes the resized window to flash repeatedly by disabling the ability to run while resizing. (Aceearly1993)     

#### [1.4.2] - 2024/2/19 #### 

(Shared)  
`FIXED` - Some Map chip layering errors at Rivoire Cave.  (Aceearly1993)  
`FIXED` - A bug to text size after resizing the windows display scale to be higher than 100%. (Aceearly1993)  
`CHANGED` - In-depth adjust of text formats to fit screen resize situations. (Aceearly1993)  
`ADDED` - Regulations in keyboard remap function so that hardcoded system keys won't get accidently recognized as valid input in keyboard remap. (Aceearly1993)  
`CHANGED` - Terminated the mentioning of small keyboard region due to redundant.  (Aceearly1993)  
`ADDED` - Regulations in keyboard remap function so that multiple keyboard keys won't get registered the same key function. (Aceearly1993)  
(Catoblepas)  
`ADDED` - Port the Gorgon 1.4.1 changes to graphic variations to Catoblepas builds (1.4.0). (Aceearly1993)  
(Gorgon)  
`FIXED` - A bug that causes the capability of air dash to be temporarily locked up after performing a chain of air dash>sword attack actions. (Aceearly1993)  


#### [1.4.1] - 2024/1/15 #### 

(Gorgon build only)  
`ADDED` - Simplified Chinese and Japanese variation of misc. enemy bestiary embedded text.  (Aceearly1993)  
`ADDED` - Enemy description (currently only in English/Simplified Chinese). (Aceearly1993)  
`ADDED` - Simplified Chinese variation of boss rush character selection screen embedded text. (Aceearly1993)  
`CHANGED` - In-depth adjust of text formats in enemy bestiary screen to fit localizations. (Aceearly1993)  


#### [1.4.0] - 2024/1/10 #### 

`CHANGED` - Mini Map: The red ghost rooms will now be marked in a different color scheme, which makes them more recognizible on mini map. (Aceearly1993)  
`CHANGED` - Garden of the Dead: Make the A-letter panel temporarily blink in order to reduce progression problem. (Aceearly1993)  
`ADDED` - More new event notes and restored more event notes from source document file regarding the changed parts.  (Aceearly1993)  

#### [1.3.9] - 2023/12/29 #### 

`CHANGED` - Direct X 9: Bold settings and text format to prevent pickup item text (CHS/JPN) from clipping out of text box on some computers. (Aceearly1993)   
`CHANGED` - Direct X 9: Tweak and adjusts to prevent weapon/equipment text - pause menu (CHS/JPN) from clipping out of text box on some computers. (Aceearly1993)  

#### [1.3.8] - 2023/12/25 #### 

`CHANGED` - Ditch red text variations for better visibility. (Aceearly1993)  
`CHANGED` - La Tourvelle castle: Coloring on a ring object for better visibility.  (Aceearly1993)  
`CHANGED` - Tweak and adjusts on descriptions in readme. (Aceearly1993)  
`CHANGED` - Minor position tweak on Simplified Chinese text embedded as pictures - Monster chart screen/Teleport spots. (Aceearly1993)  


#### [1.3.7] - 2023/12/20 #### 

`FIXED` - A bug carried from LC1 which will cause invincibility potion timer HUD to be gone after a scene swap.  (Aceearly1993)  
`FIXED` - Several text corruptions in multilanguage texts that can only be seen on Direct X 11 mode.  (Aceearly1993)  
`ADDED` - More event notes.  (Aceearly1993)  
`ADDED` - Direct X 11 counterpart of text events.  (Aceearly1993)  
`ADDED` - Video option application for VSync toggle. (Aceearly1993)  
`CHANGED` - Reorganized text events that will be affected by Direct X 11 mode.  (Aceearly1993)  
`CHANGED` - Slightly tweaked JPN/CHS text phrasing for Direct X 11 mode.  (Aceearly1993)  
`REMOVED` - A global event in jumping sound that will cause sound bugs. 
The adjust of sound volume jumping sound will be predefined in sound clip instead of being adjusted through events.   (Aceearly1993)  


#### [1.3.6] - 2023/12/11 #### 

`ADDED` - More event notes. (Aceearly1993)  
`CHANGED` - Load method of Sounds to improve loading time when changing scenes. (Aceearly1993 & Mig)  


#### [1.3.5] - 2023/11/9 #### 

`FIXED` - A very rare occasion that can cause out of bound by a side effect of mapchip position rework. (Aceearly1993)  
`CHANGED` - Sound volume of jumping sound. (Aceearly1993)  
`ADDED` - One more event as an attempt to rule out a bug (an extremely rare variation of Dual Shock 4 input stuck bug) and hope this time the bug can be removed once and for all. (Aceearly1993)  


#### [1.3.4] - 2023/11/1 #### 

`FIXED` - Inconsistency regarding animation of Skeleton gunman enemy. (Aceearly1993)  
`FIXED` - Debug command key position to reduce overlapping with main keyboard region. (Aceearly1993)  
`FIXED` - Make Debug command keys permanently disabled instead of just not immediately loaded. (Aceearly1993)  
`FIXED` - One overlap within debug position warp command.  (Aceearly1993)  
`FIXED` - One collision bug of platform in Rivoire Cave which will make backtracking difficult for wrong reason.  (Aceearly1993)  
`ADDED` - Backported invincibility potion timer from LC1. (Aceearly1993)  
`ADDED` - More event notes for better visibility to future editors. (Aceearly1993)  
`ADDED` - Controller support to a hidden easter egg screen to reduce confusion and inconvenience. (Aceearly1993)  
`ADDED` - Simplified Chinese text variant for keyboard direction keys remapping. (Aceearly1993)  
`CHANGED` - Reorganized gamepad control event. (Aceearly1993)  


#### [1.3.3] - 2023/10/29 #### 

`FIXED` - Font bugs of Japanese and Simplified Chinese texts in Delbasee City and Guernon University after changing the fonts. (Aceearly1993)  
`FIXED` - A note in Simplified Chinese texts - Garden. (Aceearly1993)  
`FIXED` - A minor layering problem at Albaret earldom overlooked in previous checks. (Aceearly1993) 


#### [1.3.2] - 2023/10/26 #### 

`ADDED` - Jumping environmental sounds ported from Wallachia. (Aceearly1993)  
`ADDED` - Recovered original notations in Alucard's animations for better visibility to future editors. (Aceearly1993)  
`ADDED` - Simplified Chinese variant in a hidden easter egg screen. (Aceearly1993)  
`ADDED` - Simplified Chinese variant in a secret screen. (Aceearly1993)  
`FIXED` - Inconsistency with Alucard's new walking animations, new jump animation and relative air animations. (Aceearly1993)  
`FIXED` - Size and position of Character art in a secret screen. (Aceearly1993)  


#### [1.3.1] - 2023/10/24 #### 

`CHANGED` - Control config screen formatting and layout. (Katriel & Aceearly1993)  
`CHANGED` - Discarded the changes in 1.3.0; Isolate No V-Sync into a separated build (the mechanic is incompatible with LC2 structure and can make confusions.) (Aceearly1993)  


#### [1.3.0] - 2023/10/21 #### 

`HOTFIX` - Implemented toggle V-Sync on/off trigger in Global event. (Aceearly1993)  

- F6 - Toggle V-Sync on/off

`ADDED` - Notation of V-Sync on/off trigger at video mode screen. (Aceearly1993)  


#### [1.2.9] - 2023/10/20 #### 

`FIXED` - A design oversight in original which causes you to accidently lost a recover potion by using such recover potion when Efrain's HP is already full. (Aceearly1993)  
`ADDED` - More event notes for better visibility to future editors. (Aceearly1993)  
`ADDED` - Localized counterpart of "Ring of Fury mode" embedded texts. (Aceearly1993)  
`ADDED` - "Ring of Fury mode" embedded texts in pause menu as indication when you're currently in gameplay of Ring of Fury mode. (Aceearly1993)  
`CHANGED` - Color brightness of "Ring of Fury mode" texts for better visibility. (Aceearly1993)  
`CHANGED` - Translate rest of untranslated parts in Simplified Chinese and Japanese counterparts in pause menu to match the translation quality in Chronicles of the Wolf. (Aceearly1993)  
`BETA` - Situation of Windows Vista compatibility to be identical to original. (Aceearly1993)  


#### [1.2.8] - 2023/10/15 #### 


`FIXED` - Inconsistency of spacing in Japanese item pickup dispaly textbox. (Aceearly1993)  
`FIXED` - Inconsistency of two map tiles in Albaret.  (Aceearly1993)  
`FIXED` - Two errors in Japanese script.  (Aceearly1993)  
`FIXED` - More notes for better visibility to future editors. (Aceearly1993)  
`CHANGED` - Japanese font for better visibility.  (Aceearly1993)  
`CHANGED` - Optimization: Fuse windowed mode input stuck fixes into global events.  (Aceearly1993)  
`CHANGED` - La Tourvelle Castle: Copied the trigger action to unused hint to the front of another indoor roman number plate.  (Aceearly1993)  



#### [1.2.7] - 2023/10/10 #### 

`FIXED` - Inconsistency of Alucard's new walking animation.  (Astral "Bozo" Clocktower)  
`FIXED` - Inconsistency of Alucard's jumping/falling animation.  (Aceearly1993)  
`FIXED` - "Do not use as function keys" text position for multi language.  (Aceearly1993)  
`FIXED` - Better Compatibility of Simplified Chinese and Japanese texts on different computers; preparation of Direct X 11 compatibility port.  (Aceearly1993)  
`FIXED` - Blocked an extremely rare variation of Dual Shock 4 input stuck bug that was missed from previous checks - by adding 3 more rules.  (Aceearly1993)  
`ADDED` - Most notations of subjects that demanded future changes in event editor, for visibility convenience of any future editor if one day Aceearly1993 is in absence.  (Aceearly1993)  
`ADDED` - Hint text of one puzzle unused in original.  (Aceearly1993)  
`CHANGED` - Hidden esater egg's input detection so that the adding of alterable value counter is now only accepted in "main screen visual" region;   
Changed the key to trigger it for avoiding input confusion;   
Changed key press count to 8 times to make the triggering easier.  (Aceearly1993)  
`CHANGED` - One text in red room in order to fit the situation if you intended to miss the ghost for the first time (example: in all relics speedruns).  (Aceearly1993)  
`CHANGED` - Simplified Chinese embedded text color in sub menu.  (Aceearly1993)  
`CHANGED` - Font type of "controller type" and "Do not use as function keys" texts for multi language;
Adjusted positions of "please refer to LC2 Github pages" texts.  (Aceearly1993)  
`CHANGED` - Nerf the addition damage scaling dealt in following situations:
- Damage taken during aura blast charging. 
- Damage taken during "Weak" status.  (Aceearly1993)
  
`CHANGED` - Made Gale Headband's function (reduce heart consumption) more effective. (Aceearly1993)  
`CHANGED` - In load file screen/boss rush result screens, Simplified Chinese and Japanese texts now have unique afonts where they have to share with Western text paragraphs in the same text object. (Aceearly1993)  
`REMOVED` - Duplicated stage tile map in La Tourvelle for optimization.  (Aceearly1993)



 #### [1.2.6] - 2023/9/29 #### 

`HOTFIX` - A bug that makes the font for pickup item display texts return to their default value rather than using the pre-determined fonts upon entering the sub menu/map screen and quitting.  (Aceearly1993)  



 #### [1.2.5] - 2023/9/28 #### 

`FIXED` - Alucard Jump animation inconsistency.  (Aceearly1993)  
`CHANGED` - Alucard walking animation. (ACC (a.ka."得枫.德广"))  


 #### [1.2.4] - 2023/9/20 #### 
 
`RETRIEVED` - Source document file for the game. (Mig)  
`FIXED` - Some issues in Spanish text.  (Aceearly1993)    
`FIXED` - Some issues in Italian text.  (Aceearly1993)    
`FIXED` - One inconsistency part in French text script.   (Aceearly1993)    
`CHANGED` - Groups of Control input events are made combined into Global event for optimization. (Aceearly1993)    
`FIXED` - Blocked an extremely rare variation of Dual Shock 4 input stuck bug that was missed from previous checks by adding one more rule. (Aceearly1993)    
`FIXED` - Re-implemented notes for item pickup events. (Aceearly1993)    


 #### [1.2.3] - 2023/9/1 #### 

`ADDED` - Brazilian Portuguese variation of reworked text script.  (Aceearly1993)  
`ADDED` - Picture variant of Efrain and Alucard if player gets "Best" rank in boss rush. (Aceearly1993)  
`FIXED` - General missing parts in Portuguese text script.   (Aceearly1993)  
`FIXED` - One inconsistency part in Simplified Chinese text script.   (Aceearly1993)  
`CHANGED` - In-depth adjust of Alucard player walking animation's speed. (Aceearly1993)  


 #### [1.2.2] - 2023/8/27 #### 


`ADDED` - Brazilian Purtuguese variant of stage name title graphics missing in original.  (Aceearly1993)  
`ADDED` - Simplified Chinese and Japanese variant of resist negative status rate text to match the localization quality in Chronicles of the Wolf. (Aceearly1993)  
`FIXED` - One Brazilian Purtuguese text error not caught previously for some reason. (Aceearly1993)  
`CHANGED` - Updated PoV (PS4) direction control system and Controller Recognition system to V1.3; 
Fully separated inputs of Keyboard, Xbox controller and PS4 controller/PoV direction input into 3 groups as an attempt to prevent control stuck bugs and overrides.  (Aceearly1993)  
`CHANGED` - If the game window is not focused, the game now temporarily disables Xbox D-pad controls 
(as an attempt to prevent control stuck bugs introduced after implemented PoV direction controls if going across "loading" zones when the game window is not active). (Aceearly1993)  
`CHANGED` - Forced the game to always keep V-Sync active to prevent performance issues. (Aceearly1993)  
`CHANGED` - One instance of German variant of stage name title graphics for consistency with new translations. (Aceearly1993)  
`FIXED` - An issue that the game will lose control in PoV direction control (Xbox controller) after going across brief "loading" screens if temporarily deactive the game window; 
This is fixed by isolating Xbox D-pad inputs to be exclusively in Xbox gamepad controls. (Aceearly1993)  


 #### [1.2.1] - 2023/8/17 #### 


`ADDED` - Rest of language variations of item/equipment name when items/equipment are picked up in action scene. 
This is done to match up the localization quality of all western languages in Chronicles of the Wolf. (Aceearly1993)  
`ADDED` - Rest of language variations of item/equipment name in Sub screen > monster chart section. 
This is done to match up the localization quality of all western languages in Chronicles of the Wolf. (Aceearly1993)  
`ADDED` - Misc. object icon for text objects related to monster chart and pick up item display text box. (Aceearly1993)  
`ADDED` - A simple background to make the control config screen and boss rush character selection screen look less barebone. (Aceearly1993)  
`ADDED` - The function that can auto detect game pad type from demo version of Wallachia. (Aceearly1993)  
`FIXED` - An oversight in original that will cause the initial map index to go wrong in Servigny Mansion's save spot. (DragonX24)  
`FIXED` - A text corruption in Italian script not previously caught for some reason. (Aceearly1993)  
`FIXED` - Several background positioning errors in St Justine. (Aceearly1993)  
`FIXED` - Several background positioning errors in Garden of the Dead. (Aceearly1993)  
`FIXED` - Servigny earldom: A layering error at the left side of Azure Lake so that it's now identical to original. (Aceearly1993)  
`FIXED` - Revamped the Controller recognization system to get rid of several issues:  
              1. An input stuck bug when a direction of Xbox d-pad is pressed if window is not focusing.  
              2. A control problem when directly jumping to scene frames through frame editor if an Xbox d-pad is plugged.  (Aceearly1993)  
`CHANGED` - Garden of the Dead: Slightly tweaked a sentence in a French text object in order to fit the text box graphics better. (Aceearly1993)  
`CHANGED` - Auberge/Dark Forest: Tweaked some graphics for better visibility (done by requests of CHS people). (Aceearly1993)  



 #### [1.2.0] - 2023/8/3 #### 


`ADDED` - Simplified Chinese and Japanese variation of item/equipment name when items/equipments are picked up in action scene. 
This is done to match up the localization quality of CHS/JPN languages in Chronicles of the Wolf. (Aceearly1993)  
`FIXED` - An oversight in original that the chosen Language selection in title screen menu did not get saved in the config file immediately. 
This is done to match up the program's quality in Chronicles of the Wolf. (Aceearly1993)  
`FIXED` - A bug that will cause stage name title in boss rush to repeatedly appear upon walking back and forth on the area transition line between initial preparation room and first boss room.  (Aceearly1993)  
`CHANGED` - Slightly Reworked the structure of pickup name display code region for better visibility if any future editor want to take on improvement on other languages for this section.  (Aceearly1993)  
`CHANGED` - Monster chart: One instance of Japanese variation of max up item name texts for consistency to Original languages. (Aceearly1993)  
`CHANGED` - Relic Description: Several instances of Japanese variation of Silver Statue name texts for their new variants with better placing on pickup text box. (Aceearly1993)  
`CHANGED` - Font: Item pickup text box font to cover an issue that causes the new Japanese variant of Item pickup text to exceed the text box in rare circumstances. (Aceearly1993)  
`CHANGED` - Reworked video options so it's once again functional. The reworked video options screen has more functions and included brief indicators for every function. (Aceearly1993)  
`CHANGED` - Font size of Keyboard key indicator display in controls setting for better visibility. (Aceearly1993)  



 #### [1.1.5] - 2023/7/28 #### 


`ADDED` - Simplified Chinese and Japanese variation of stage name title. (Aceearly1993)  
`ADDED` - Rewritten Controller Recognization system to erase a bug ONLY in Xbox type Controller following the inclusion of Point of View control. (Aceearly1993)  
`FIXED` - A Japanese translation error in one of the original embedded pictures.  (Aceearly1993)  
`CHANGED` - Build method Defaults to "unpacked exe" as an attempt to reduce the risk of rising malware false positive flag. (Aceearly1993)  
`CHANGED` - Font style of several Simplified Chinese and Japanese texts for better visual. (Aceearly1993)  


 #### [1.1.4] - 2023/7/22 #### 


`ADDED` - More Info of Reworked Edition Credits. (Aceearly1993)  
`ADDED` - The fix of DualShock 4 D-pad compatibility to every Point of View direction to better reduce confusion. (Aceearly1993)  
`FIXED` - Clean up of equipment name consistency.  (Aceearly1993)  
`FIXED` - The remaining bugs caused by adding DualShock 4 D-pad compatibility to the game. (Aceearly1993)  
`CHANGED` - When you exit from Boss Rush result screen, there will be fade transitions instead of abruptly changing to reset command. (Aceearly1993)  

 #### [1.1.3] - 2023/7/19 #### 
 
`ADDED` - Source document of Spanish translation texts. (Jorge. D. Fuentes)  
`FIXED` - The rest on inconsistence in Spanish translation. (Aceearly1993)  
`FIXED` - A bug related to DualShock 4 D-pad compatibility that the game's keyboard control will go awry if a gamepad is not plugged in. (Aceearly1993)  


 #### [1.1.2] - 2023/7/15 #### 

`ADDED` - DualShock 4 D-pad compatibility. (Mig & Aceearly1993)  
`ADDED` - Alternate exe build generated by Clickteam Fusion 2.5+ developer along with regular 2.5 developer for experiments. (Aceearly1993)  



 #### [1.1.1] - 2023/7/6 #### 


`ADDED` - Unique German variant of "do not use (KEYS) as function keys" texts. (Aceearly1993)  
`ADDED` - Readme will have a (optimized) Simplified Chinese variation. (Aceearly1993)  
`FIXED` - Several typos in Spanish translation. (jdbuenol)  (1000/3342 WIP)  
`FIXED` - Several typos in German translation. (Exorion Hagen)  
`FIXED` - Managed to find and fix more tile errors throughout the game. (Aceearly1993)  
`FIXED` - More object icons in frame editor to be identical to the object icons in the mask data of the demo.  (Aceearly1993)  
`CHANGED` - Graphics of Title screen date info.  (Katriel & Aceearly1993)  
`CHANGED` - Graphics of equipment menu in order to be consistent with the German translation fix. (Aceearly1993)  



 #### [1.1.0] - 2023/6/29 #### 

`ADDED` - Unique area name picture of Boss Rush. (Aceearly1993)  
`ADDED` - Unique Simplified Chinese and Japanese variant of monster chart texts.  (Aceearly1993)  
`ADDED` - Unique Simplified Chinese and Japanese variant of "do not use (KEYS) as function keys" texts. (Aceearly1993)  
`ADDED` - Unique Simplified Chinese variant of boss lifebar name. (Aceearly1993)  
`ADDED` - Fade out effect when you either completed a boss rush character selection or exit from Boss Rush character selection screen. (Aceearly1993)  
`ADDED` - Notes in readme regarding antivirus stuff. (Aceearly1993)  
`ADDED` - More properties info for the game in order to reduce the chance of being targeted as malware by antivirus programs. (Aceearly1993)  
`FIXED` - Tile Layering mistakes in Boss Rush area. (Aceearly1993)  
`FIXED` - Graphic error in a map chip in La Tourvelle area. (Aceearly1993)  
`FIXED` - Managed to find and fix more tile errors throughout the game. (Aceearly1993)  
`FIXED` - More object icons in frame editor for visibility. (Aceearly1993)  
`FIXED` - Control Bugfixes. (DragonX24)  
`CHANGED` - Title screen mist is a bit closer to original.  (Aceearly1993)  
`CHANGED` - Slightly tweaked the format of monster chart section in event editor for better visibility if any future translator want to proceed the localization improvement task.  (Aceearly1993)  
`CHANGED` - When you exit from Boss Rush character selection screen, the game will go back to main title screen instead of reset. (Aceearly1993)  


#### [1.0.1] - 2023/6/8 #### 

`FIXED` - A bug where the control config object is receiving valid input from main title screen. (Katriel & Aceearly1993)  


#### [1.0.0] - 2023/6/8 #### 

`RELEASE` - Initial release!!!!!!



#### [0.9.3] - 2023/6/8 #### 

`FIXED` - Tile Layering mistakes in the teleport rooms and albaret areas in original. (Aceearly1993)  
`FIXED` - A text box graphic error at the "choose your own death" room in S.Chinese. (Aceearly1993)  


#### [0.9.2] - 2023/6/7 #### 

`ADDED` - Description of "LC2_KeyBinding.ini" in the readme files. (Aceearly1993)  
`CHANGED` - Minor adjust to S.Chinese embedded text in game over screen. (Aceearly1993)  
`CHANGED` - Deleted "S.Alucard" (the development leftover, which contains Alucard's SotN sprite template) in St.Justine for reducing potential of receiving DMCA harshment. (Aceearly1993)  
`FIXED` - A bug related to non-ASCII letter input by disabling the function to switch to non-ASCII IME in-game. (Aceearly1993)  
`FIXED` - "Whitered" typo in monster guide section of the .txts. (Aceearly1993)  


#### [0.9.1] - 2023/6/6 #### 

`ADDED` - "LC2_KeyBinding.ini" in the release tag. (Aceearly1993)  
`CHANGED` - Re-enabled small keyboard region controls for those who happened to prefer small keyboard region. (Aceearly1993)  
`CHANGED` - The alternate pause key (plays jingle and the screen stays still when paused) from "Space bar" to "Esc" in order to not interfere the new default keyboard control. (Aceearly1993)  
`CHANGED` - "Guide" screen UI to reflect the hotkey changes. (Aceearly1993)  
`FIXED` - An issue where the keyboard control in "true start screen" did not work if start the game in a fresh new location where the "LC2_KeyBinding.ini" is not generated yet. (Aceearly1993)  
`FIXED` - Minor display issue in various Brazilian-Portuguese texts. (Aceearly1993)  
 

#### [0.9.0] - 2023/6/5 #### 
`ADDED` - Last bit of missing Brazilian-Portuguese texts and pictures. (Aceearly1993 & Katriel)  
`ADDED` - Japanese and S.Chinese now have unique monster guide enemy name counterpart instead of sharing the default English counterpart. (Aceearly1993)  
`CHANGED` - Keyboard remapping plugin and related logic. Hopefully the character stuck problem could be gone. (DragonX24)  
`CHANGED` - Adjusted sub menu description font in Japanese once again for consistency. (Aceearly1993)  
`REMOVED` - Default Small keyboard region control, and its reference in task bar. (Not necessary anymore.) (Aceearly1993)  
`REMOVED` - Mute music and Mute samples hot key function in the framework of original game in order to avoid confusion caused by misinput in keyboard control. (Aceearly1993)  
`FIXED` - An issue where the exit button did not work in boss rush mode character selection. (Aceearly1993)   
`FIXED` - Unique icon of plain text object for better visibility in frame editor. (Aceearly1993)   
`FIXED` - Several typos in monster guide entry. (Aceearly1993)   
`FIXED` - Several graphical errors throughout the in-game areas.  (Aceearly1993)   
`RELEASE` - Soft-release the version to Chinese and Japanese communities for Chinese translation quality check and feedbacks. Hopefully the very last major update before the 1.0 release. (Aceearly1993)


#### [0.8.0] - 2023/6/1 #### 

`ADDED` - Missing counterparts of brazilian-portuguese texts and pictures. (Aceearly1993 & Katriel)  
`CHANGED` - Two instances in Japanese script for consistency of second personel. (Aceearly1993)  
`CHANGED` - Soft reset command from F2 key to Ctrl+F2 key to avoid accident misinput. (Aceearly1993)  
`CHANGED` - Description ("Guide") screen UI to reflect global function hotkey changes. (Aceearly1993)  
`FIXED` - Unique icon of plain text object for better visibility in frame editor. (Aceearly1993)  
`FIXED`  - An attempt to address issues with frame speed in Alucard player's walking animation. (Aceearly1993)  
`FIXED`  - Graphic error in the Alucard event animation in St. Justin. (Aceearly1993)  
`FIXED`  - Issues with consistency of distances between text at S.Chinese title menu. (Aceearly1993)  
`FIXED`  - Finalized and restored unused brazilian-portuguese variant of teleport room embedded texts. (Aceearly1993)  



#### [0.7.4] - 2023/5/28 #### 

`ADDED` - Recovered all brazilian-portuguese original dialogue, as well as fixed several issues and mistranslations.  
`FIX` - Wrong images on some shops.  
`FIX` - Brazilian-portuguese text alignment.  

#### [0.7.3] - 2023/5/17 #### 

`ADDED` - A task bar system which can be freely toggled on/off by pressing F8 key, previously only seen in an early demo of the game, and LC1.   

The option menu bundled within this task bar, has a built-in control option which can change the secondary variant of keyboard direction key mapping to anywhere else (There's no character stuck bug in the secondary keyboard direction key mapping), effectively countering the keyboard control bug as a temporary solution until we solved in-game control mapping bug in Mig's bottom-level code system in the future.    

#### [0.7.2] - 2023/5/16 #### 

`FIXED` - Small Keyboard region Control in save room.

#### [0.7.1] - 2023-05-16

`ADDED` - Small keyboard region control inspired from the original.  (Aceearly1993)  
`ADDED` - Extended Readme.  (Aceearly1993)  
`ADDED` - Japanese variant of "super load" screen area name text. (Aceearly1993)  
`CHANGED` - Reverted font of equipment name back to original. (Aceearly1993)  
`CHANGED` - Japanese and Simplified Chinese language variants now use unique font for equipment name. (Aceearly1993)  
`CHANGED` - One instance in S.Chinese script. (Aceearly1993)  


#### [0.7.0] - 2023-05-14

`ADDED` - Support of custom keyboard key rebind (WIP; contains bugs). (DragonX24)  
`ADDED` - Simplified Chinese language variant. (Aceearly1993)  
`ADDED` - Reworked version credit at credit roll. (Aceearly1993)  
`CHANGED` - Several instances where the original Japanese script fits better than the retranslated script. (Aceearly1993)  
`CHANGED` - Several instances where the embedded Japanese text as pictures need to be retranslated. (Aceearly1993)  
`CHANGED` - Config screen UI to reflect DragonX24's custom keyboard key rebind. (Aceearly1993)  
`CHANGED` - Language selection screen UI to reflect the addition of Simplified Chinese. (Aceearly1993)  
`CHANGED` - The required amount of a key press to active an easter egg from 3 times to 12 times in order to avoid confusion during keyboard key remapping. (Aceearly1993)  
`REMOVED` - Function of directly quitting the game with Esc key. Too annoying in various circumstances and is blamed by too many people. (Aceearly1993)  
`FIXED` - Several instances where the required map chip is missing in Sautelle Cemetery and Garden of Dead in original. (Aceearly1993)  

This version also introduces a bug due to new keyboard remap system, we are still trying to fix it:  
`BUG` - There's a random 1/2 chance in large area transitions that Efrain sometimes won't change animation and continue to go on to the direction he was going or doing whirlwind even if you aren't pressing a button. (Keyboard control only; joypad control is not affected.)  


#### [0.6.3] - 2023-04-10

`ADDED` - Recovered Spanish and German script on the repository.  
`ADDED` - Several instances where the dialogue is missing from German text.  
`FIXED` - Position of most German plain-text.    
`FIXED` - Several German text alignments.    
`FIXED` - Most of German character font.    

#### [0.6.2] - 2023-04-09

`ADDED` - Several instances where the dialogue is missing from Spanish text.  
`FIXED` - Position of most Spanish plain-text.    
`FIXED` - Several Spanish text alignments.    
`FIXED` - Most of Spanish character font.    


#### [0.6.1] - 2023-04-08

`FIXED` - Some instances of French text corruption fixes that did not get applied in-game for some reason.    
`FIXED` - Several French text alignments.    
`CHANGED` - Text font of Weapon/Armor name text groups in Sub Screen; This is done to make Sub Screen text looks better in Japanese although the original font style of English/French/etc.. for those text groups, is sacrificed. We're sorry but this change has to be done.   
`CHANGED` - Font of most Japanese texts that stores separately from texts of other languages.   
`CHANGED` - Several Japanese lines that get affected by the changed text font.   


#### [0.6.0] - 2023-04-07

`ADDED` - Recovered Italian script on the repository.   
`ADDED` - One instance where the dialogue is missing from French text.  
`ADDED` - One instance where the dialogue is missing from Italian text.  
`FIXED` - Position of most Italian plain-text.    
`FIXED` - Most of Italian character font.    
`FIXED` - A typo in Italian script where the area names of Ancient Library and Servigny Mansion in "super load" screen is misplaced.   
`CHANGED` - Several instances where the Italian text won't match what the voice actor is speaking.    
`CHANGED` - The Simplified Chinese txt file coding for better visibility on GitHub.  
`CHANGED` - Some area names in Simplified Chinese txt file to match Japanese translation.  


#### [0.5.1] - 2023-04-04

`ADDED` - Recovered French script on the repository.  
`FIXED` - Position of enemy name tag large text in enemy chart.  
`FIXED` - Position of most French plain-text.  
`FIXED` - Most of French character font.  
`CHANGED` - Two instances where the Japanese text would exceed the dialogue box.  

#### [0.5.0] - 2023-04-03

`ADDED` - Reintroduced V-Sync to get rid of framerate problems on newer computers.  
`ADDED` - Basic info of the game's original developer.  
`FIXED` - Position of most Japanese text.  
`CHANGED` - Japanese translation; it now uses the re-translated script for plain-text parts.  

#### [0.4.1] - 2023-03-29

`ADDED` - Languages in progress on the repository.  
`FIXED` - Transparency: water droplets on Ice Cave, glass prices on Horror Gallery and tubes on Castle Clockwork.  
`FIXED` - La Tourvelle Castle area name not showing up.  

#### [0.4.0] - 2023-03-12

`ADDED` - Reintroduced text anti-aliasing.  
`FIXED` - Some transparent effects: Bubble enemies and its projectiles, rain and broken glass on Nightmare plant.  
`FIXED` - Some typos on english text.  

#### [0.3.4] - 2023-03-06

`FIXED` - Snowfall transparency effect.  
`FIXED` - In game music, so it behaves like the original and don't get cutted.  
`FIXED` - Music at character selection on boss rush screen.  

#### [0.3.3] - 2023-03-06

`FIXED` - Anna's transparency veil.  
`FIXED` - Color of last unique event teleporter.  

#### [0.3.2] - 2023-03-05

`FIXED` - More reported transparency error.  

#### [0.3.1] - 2023-03-05

`FIXED` - One name on english credit text.  
`FIXED` - Centered a few text lines on boss rush and new/loading file.  

#### [0.3.0] - 2023-03-04

`FIXED` - All english text.  
`FIXED` - Fog on entrance of Castle of Eternal Night in Albaret.  
`FIXED` - Center aligned current saving location on loading file.  

#### [0.2.1] - 2023-02-28

`FIXED` - More transparency errors related to enemies.  
`FIXED` - Most if not all illumination effects.  
`FIXED` - Fullscreen bug on music box.  
`FIXED` - Center aligned boss rush and HUD text.  

#### [0.2.0] - 2023-02-26

`CHANGED` - How trasparency works, it should behave more like the original.  
`FIXED` - More transparency errors.  
`FIXED` - Some illumination effects.  
`FIXED` - In game timer never moved foward.  
`FIXED` - Centered wrongly aligned text.  
`FIXED` - Warp room wrong color.  

#### [0.1.1] - 2023-02-25

`CHANGED` - Keep sounds when unfocused for better streaming experience <sup>(Recommended by Jupiter Climb)</sup>  
`CHANGED` - Dafault controller of the first player to joystick 1  
`FIXED` - Most if not all reported water/dark transparency effects should be fixed  
`NEW` - Full english dialogue is available in the repository  

#### [0.1.0] - 2023-02-22

`REMOVED` - Support for DirectX 8, only DirectX 9 and up are now supported.  
`FIXED` - Several water areas opacity problems.  
`FIXED` - A few transparency effects on waterfalls and fogs.  
`FIXED` - Some problems day/night cycle shading effects caused by DirectX 8.  
`FIXED` - Some text alignment on saves and new/load game screen.  

#### [0.0.2] - 2023-02-21

`ADDED` - New icon on application  
`CHANGED` - Reworked screen resolutions and windowed mode, video options won't work anymore.

#### [0.0.1] - 2023-02-20

`START` - Project began here! 🎉

## Thanks
- Migami Games
- Konami
- Robert Belgrade
- palmymkgames
- Aceearly1993
- DragonX24 (https://www.projectdread.com/) - Reworked Keyboard function
- mashedpotatoes312
- theplottwist
- Jorge. D. Fuentes
- jdbuenol
- Exorion Hagen
- 狼王之2型 (https://space.bilibili.com/936194) (Japanese re-translation)
- ACC (a.k.a."得枫.德广")(https://space.bilibili.com/1471923), Astral "Bozo" Clocktower (Alucard animation enhance)  
... and all the people in game credits.
