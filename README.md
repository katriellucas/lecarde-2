# The LC2 Rework Project

![20250409095910](https://github.com/user-attachments/assets/0e346364-0437-4acb-b212-6ffd27f8c0fc)


## Description
Source code of the fan-game Castlevania: The Lecarde Chronicles 2 made by Migami Games. Due to a HDD failure, the original source have been lost. This repo is an atempt to preserve, fix and improve this game.

Unfortunately, the recovery process ended up corrupting all non-English characters, many transparency effects and more. So, if you know any of the following languages and is interested in helping us out by fixing and re-translating this project, feel free to contact us, we are in need of:
- Someone who're both good at Clickteam Fusion 2.5 and good French speakers (preferably)
- Someone who're good at Clickteam Fusion 2.5


## Disclaimer
We contacted Migami Games and got approval to keep this repository up.  

The release of Lecarde Chronicles 2 got permitted by Konami, the game and its assets are freeware and **_SHOULD NOT_** be sold, this also includes the source code. Any modifications you do have also to be free. Castlevania is an intellectual property owned by Konami, please support the company by buying their official releases. 


## Usage

![20250409100057](https://github.com/user-attachments/assets/04215660-cfe0-4b11-9674-e89973b8a84e)

To get the reworked game builds, go to "Releases", choose the latest "v*. *. *-alpha" tag and find the .exe files in the "Game Binary" zipped file. The .exe file is the generated executable, while the .mfa file in "Source Code" zipped file fis the (recovered) Clickteam Fusion project file necessary to generate the .exe (note in this game's case, it requires some extensions from Clickteam Fusion 2.5 Developer builds to be opened). 


The "Alternate build method" branch is only needed if the initial build method did not work.

The "native aspect ratio stretched" branch is only needed if you did not like the intended aspect ratio (force 4:3).

They are put there only to fulfill more personal preferences that a lot of people demanded them.


Note that the original game is infamous for the compatibility issue for PS4/Xbox controllers if your computers are unlucky so it left the controller preference blank. Here's a valid workaround to this issue if you encountered it like us:

In Control Panel→ Devices and printers, find PS4 controller (usually labeled as "Wireless Controller"), right click "Wireless Controller" label to find controller setting, then click "advance..." to go into advance setting of "Wireless Controller", and be sure the "Wireless Controller" is checked as the preference.

The same could be applied to Xbox Controllers by repeating the setup above while your desired Xbox controller is plugged in.

If your controller is NS type we cannot guarantee if it works 100% (too much problems with the game's bottom structure) but we provided baseline support and NS type controller label anyway.


#### PC Specification Requirements #### 

CONFIGURATION:   
(Based upon vanilla game's DX9 mode)   
System OS: Windows XP / Vista / 7 / 8 / 10   
Processor: Intel Core2Duo 2.20GHZ or higher - Memory 1GB  Ram-   

500 MB free Hard drive space   
Video Card: Direct 3D9 Compatible   


#### Read this if you encountered random crash exit when pausing #### 

![LC2](https://github.com/user-attachments/assets/c7aabe0e-0d57-4cc4-b29b-f8eda4737d0a)


It may or may not have something to do with system compatibility, but make sure you have all the font installed which the game demanded:

Arial Unicode MS (DX11)  
Baskerville Old Face (DX9)  
MS UI Gothic  
Tahoma   
Old English Text MT (DX9)  
Bookman Old Style (DX9)  
Californian FB  (DX9)  
新宋体 (DX9)  
黑体 (DX9)  

If some of the fonts did not get installed in you computer, the game will be unable to find them and thus cause problems.


#### System compatibility warning #### 

The game is only verified to be working as intended on windows revisions up until Windows 10 20H2 revision. 
Beyond that revison it's out of my control and nor will there be any hope of making compatibilities specifically for the unintended system (at least from me).

If any graphical glitch occurs, please make sure your Direct X 9 or Direct X 11 dependencies is correctly installed before report as a reproduce-able bug!!!


#### About "LC2_KeyBinding.ini" #### 
![20250409100627](https://github.com/user-attachments/assets/84dd9dd7-a641-4700-9e36-e246a3e2c3be)

A reworked version of the keyboard control created by DragonX24.
This file must be placed in the same directory the game locates if you downloaded the game and moved the game files to a fresh new location.

#### NEW Hotkey Functions #### 

- Controller re-connect hotkey if auto recognization upon re-plug fails: F6

To make the game display 1:1 pixel perfect scale:
- You must make sure the display monitor's vertical size is above 1000.
- You must make sure the windows display scale is exact 100%.
- Toggle anti-alias to off after opening the game.

#### About "Alternate build method" #### 

"Alternate build method" is done as an attempt to keep a small quirk away that the core plugin components of the game might be lost depending on player's local settings of firewalls, 
but on some situations it will cause antivirus flag to go mad so not recommended unless you want to go with loyalty and purity to vanilla.


#### About "Native Fullscreen resolution" #### 

Some players did not like the intended aspect ratio for preference reasons and prefer stretched fullscreen scale so this is provided as an alternated option. 



#### Read this if antivirus softwares flagged the game as Malware ####

![20250409100426](https://github.com/user-attachments/assets/cf167b0d-96bf-4a37-ac36-0515f2281368)

It's something about Clickteam's engine itself. Antivirus softwares don't seem to be too kind towards some Games used Clickteam's engine. If the problem that the antivirus softwares flagged the game as malware occurs, either turn off the antivirus software in question, or add the game to its white list. Also avoid directly sharing the zips or folder(s) which contain the exe file unless really necessary because some net drive safety calculation like Google's, don't seem to be too happy with the game. 

#### Read this if your screen capture program did not work in Reworked LC2 ####
Some capture programs will have compatibility issue with reworked LC2 on Windows 10 (for example, Ocam). This is because the compatibility issue of some revisions of Windows 10's Direct X9 mode. If you want safe screen recording methods, more mainstream programs (like OBS) will work.


#### Read this if you encountered framerate problem in fullscreen mode #### 
1. It might be something about your setting of VSync under Direct X 9 mode. If your only graphic card is a Nvidia GTX graphic card, toggle VSync in your Nvidia control panel to "fast" or "on" if you encountered
frame rate problem in fullscreen mode.
2. It might be something with how the engine dealt with graphic rendering; Only turn V-Sync off if you encountered input lag with V-Sync on.


#### Known bugs #### 
- If the game's project file is loaded through frame editor, quickly unfocus the game window by overlapping it with a larger window upon proceeding a frame change, when the next frame about to be loaded, the cursor will automatically move upwards. We tried multiple ways but cannot proceed bright results to rule out it. This shouldn't get in the way of normal gameplay on the generated .exes, though.

- If quickly unfocus the game window when holding a direction key at title menu, then focus back, the game's direction input will stuck. This is because the reworked game requires Control X plugin to sufficiently apply newly assigned Keyboard key input dynamically (in DragonX24's remodeled key assign formula) with the structure of such plugin is unfortunately too old and can generate issues with LC2 structure. Shouldn't get in the way of normal gameplay though.

### Rules on Submitting a Translation error ###
The text script is well established in 2 years and not really a subject to be dispatched again and again; Please submit a translation error only when the errors are serious and inconsistency is huge enough. Hope we can earn your understandings.


Discuss the reworked version of Lecarde 1 and Lecarde 2:   
https://discord.gg/yuS7VjPfYM 


Discuss more Migami games works (mainly their works AFTER their transition into a commercial studio): 
https://discord.gg/uAVxVqmZXx  


## Changelog

#### [1.6.7] - 2026/9/3 #### 

`EXPERIMENT` - The joystick 2 object just received a sudden update out of nowhere. I cannot resist the temptation of any possible chance on improvements and will test the new version right in this release. (new version of object updated by NaitorStudios)  
`CHANGED` - Spotlights: Adjusted collision condition so that it's consistent to the condition used in [Chronicles of the Wolf]. (Aceearly1993)  
`CHANGED` - Pause Menu/Mini Map: Adjusted timing of the game capable to receive exit input so that it's identical to the condition used in [Chronicles of the Wolf]. (Aceearly1993)  
`CHANGED` - Pre-input of double jump/triple jump after air dash: Timing became slightly wider. (Aceearly1993)  
`FIXED` - Isigny Village: Fixed a graphic order so that main character will always be in front of the funnel. (Aceearly1993)  
`FIXED` - Eternal Light: An error in the stage name graphic so that it's more gramatically correct in German language variant. (Soul D. Sol/Aceearly1993)  


#### [1.6.6] - 2026/7/2 #### 

`CHANGED` - Main hitbox: Due to player feedback, Main character Hurtbox fully separated from main collision box; Added a new collision box and shrink down the size of main character hurtbox.  (Aceearly1993)  
`CHANGED` - L'Auberge rouge Inn: A hidden bonus changed to not disappear too soon, following the logic of other hidden bonus spots throughout the game. (Aceearly1993)  
`CHANGED` - Servigny Mansion: Minor adjust to make the Jeanne de Servigny sub-boss capable to defeat without having to take damages. (Aceearly1993)  
`ADDED` - More original event notes in the project file. (Aceearly1993)  
`FIXED` - A bug in the temporary fix of Issue #43 (related to Air Dash) where a second air dash will sometimes be lost when executed the first air dash, 
and slash in mid air before landing, then jump again and attempt to do double air dash after the next jumping. (Aceearly1993)  


#### [1.6.5] - 2026/6/18 #### 

`ADDED` - More original event notes in the project file. (Aceearly1993)  
`ADDED` - Double jump/triple jump: Added several pre-input frames so that they can be performed after an air dash much easier than before. (Aceearly1993)  
`FIXED` - An oversight in the vanilla which will cause the bones skeleton type enemies thrown to stack in object counter and not properly erased when they flied beyond the camera. (Aceearly1993)  
`FIXED` - A bug in the reworked support of Xbox triggers so that Whirlwind, air dash and air float will now be able to pull out properly with Xbox triggers. (Aceearly1993)  
`FIXED` - Garden of Deads: A bug in the collision system which will cause softlocks in unwanted situations. (Aceearly1993)  




#### [1.6.4] - 2026/5/25 #### 


`CHANGED` - Delete save file: Another sound effect will be occupied in the execution of deletion so that it will no longer be reusing the confirm sound. (Aceearly1993)  
`CHANGED` - Alucard: Added a few startup frame in Soul Steal spell animation so that it looks slightly more natural. (Aceearly1993)  
`CHANGED` - A QoL enhancement implemented so that the Invincibility potion timer/Alucard's vanish spell timer will no longer be reset by another aura blast spell. (Aceearly1993)  
`FIXED` - Main character movement: Eliminated a negative behavior which the Divine Sword aura blast motion will be broken after performing a regular slash in between charging and release motions. (Aceearly1993)  
`FIXED` - Alucard Boss rush: A graphical priority bug occured in rare circumstances that the sword object will appear in Aura Blast and Whirlwind motions where it really shouldn't. (Aceearly1993)  
`FIXED` - Garden of the Dead: Fixed a irregular behavior if for some reason you get 2 chalices before triggering the first statue's activation zone for the first time. (Aceearly1993)  
`FIXED` - Altar: Always return a variable to 0 so that the final boss trigger zone will always be possible to trigger, overriding the whatever saved variable in the save file. (Aceearly1993)  




#### [1.6.3] - 2026/3/11 #### 

`CHANGED` - Revamp the Death 2nd encounter dialogue:   
English/Portuguese/Simplified Chinese - The Lecarde 2 rework project team (Aceearly1993, ThePlotTwist, Jeffrey Montoya)  
French - Chernabogue   
Spanish - Jorge Fuentes   
German - Exorion Hagen   
Italian - Daedalus007/Shüan   
Japanese - 狼王之2型   
  
`CHANGED` - Voice files to reflect the changed Death 2nd encounter dialogue. (Jeffrey Montoya)  
`CHANGED` - Very subtle adjust to a spike in a vertical climb section at Guernon University in order to reduce player's frustration.  (Aceearly1993)  
`CHANGED` - Slide: Due to requests, unrandomized slide distance in order to end player's confusion with the game's control operation regarding slide.  (Aceearly1993)  
`CHANGED` - Melee attack: Priority of following weapons when repeatedly attacking on ground is adjusted to be more like SotN swords:
-Alucard sword when equipped by Alucard himself.  
-Light Saber, Courtoise, VV sword, Lecarde Sword.  
Also added pre-input of these weapons so that the input of a second jumping slash is less likely to get lost. (Aceearly1993)  
`CHANGED` - Added new regulations to the high-rank weapons so that the after deal of a slash can be canceled by jumping.  (Aceearly1993)  
`CHANGED` - Illusionist (boss): Post-hit flash color changed to be not aggressive. (Aceearly1993)  
`CHANGED` - Adjusted dialogue popup box position and dialogue trigger zone on some Important NPCs, in order to avoid confusions.  (Aceearly1993)  
`FIXED` - A irregular phenomenon where Aura Blast can be wrongly canceled by flipping down from platform during Aura Blast motion. (Aceearly1993)  
`FIXED` - Two typos with English text script.  (Aceearly1993)  
`FIXED` - Alucard Boss Rush: A minor inconsistency at the background effect graphic of Soul Steal spell so that the background effect graphic will
always follow the game's camera movement.  (Aceearly1993)  
`FIXED` - An inconsistency in the German script so that in equipment menu, Lecarde Sword will be displayed as "LecardeSchwert" like in pickup window instead of displaying "Lecardekilnge". (Soul D. Sol)  
`FIXED` - An oversight which the indication text of "Ring of Fury mode" will wrongly appear at file deletion screen in unwanted situations. (Aceearly1993)  
`FIXED` - A bug which the timer obj will not be hidden if you keep taking damage on spike, stationery enemies etc.. when the invincibility potion timer is about to wear off.   (Aceearly1993)  




#### [1.6.2] - 2026/2/11 #### 

`CHANGED` - Upgraded the game's engine to Clickteam Fusion 2.5+ revision 296.9.  (Aceearly1993)  
`CHANGED` - Equipment menu: Some German terms which are subjects to change in enemy description.  (Exorion Hagen)  
`CHANGED` - Hell Picture (Boss): Post-hit flash color changed to not aggressive. (Aceearly1993)  



#### [1.6.1] - 2025/11/3 #### 

`CHANGED` - Fully revamped title screen function.  
- Grouped "New Game" and "Load Game" into a single secondary screen capable to access via "Game Start" in main options along with a new "Delete save" function; 
It serves as a function to erase save file without having to manually navigate through save file's path.  (Aceearly1993)  
- Grouped "Boss Rush", "Ring of Fury Mode" and "Sound room" into a single secondary menu capable to access via "Extras" in main options.  (Aceearly1993)  
- Repositioned "Volume" into a secondary menu capable to access via "sound mode" in main options.  (Aceearly1993)  
- "Exit Game" is now reallocated at the section accessible via the same logic as other main menu options to avoid player's confusions.   (Aceearly1993)  


`CHANGED` - Nightmare Plant, Anna V.V., Death, Duke Guillecourt: Post hit flash effect changed in order to make their post-hit flash less visually aggressive.    (Aceearly1993)  
`CHANGED` - Rivoire Cave: A spot in one vertical climbing section in order to make the backtracking in Ring of Fury mode more fair. (Aceearly1993)  
`CHANGED` - Albaret Earldom: A spot in one vertical climbing section in order to make the backtracking in Ring of Fury mode more fair. (Aceearly1993)  
`CHANGED` - Sarelle Cemetery: Color of a box object in order to make it slightly more clear that it cannot be climbed.  (Aceearly1993)  
`ADDED` - Boss Rush: Quick retry function and its regulations in order to fit the latest change of title screen and reduce repetitiveness of boss rush retry.  (Aceearly1993)  
`ADDED` - Global control events: Xbox controller input added left stick detection of joystick slots 2, 3 and 4 plus their hot-replug mechanic 
in order to fit the latest update of controller detection system. (Aceearly1993)  
`ADDED` - Readme: Warning of V-sync off (experimental).  (Aceearly1993)  
`ADDED` - A trigger so that it's possible to toggle jumping sound on/off by will in order to fit player's personal preference.  (Aceearly1993)  
`FIXED` - Altar: Eliminated a negative phenomenon which decisive battle music in ending A route suddenly changed to ambiance
 if enter 3 count bosses room and immediately backtrack to ritual room before the 3 count bosses are awaken. (Aceearly1993)  
`FIXED` - Global control events: Now the game is capable to receive input from joystick slots 2, 3 and 4 instead of only capable to detect joystick slot 1. (Aceearly1993)  



#### [1.6.0] - 2025/7/16 #### 

`ADDED` - Config: Implemented on/off toggle for V-Sync and anti-alias. (Aceearly1993)  
`ADDED` - System Config: A simple global volume control added. (Aceearly1993)  
`ADDED` - Townspeople: Arrow notations on important npcs added just in case if there's any navigation issues.  (Aceearly1993)  
`ADDED` - Mini Map: Basic indicators in Castle of Eternal Night to not let newcomer player to get lost too quick.  (Aceearly1993)  
`CHANGED` - Mini Map: Color of area transition room's minimap mapchip color from green to grey in order to be consistent with the style in Chronicles of the Wolf.  (Aceearly1993)  
`CHANGED` - Mini Map: Green color will move to location of Castle's vending machine's position.  (Aceearly1993)  
`CHANGED` - Config: A secondary menu is added to hold V-Sync and anti-alias setting in video config. (Aceearly1993)  
`FIXED` - Warp zone: Several instances of Simplified Chinese text embedded as graphics. (Aceearly1993)  
`FIXED` - Item pickup: in the pickup recognization system, when [multiple heart/gold pickups of the same type/Variable were in the same spot and you touch 2 or more of them at once], 
the game will properly recognize each of them instead of only recognize once.  (Aceearly1993)  
`FIXED` - A bug of controller un-plug>re-plug trigger after 1.5.7 if controller is unplugged, proceed with keyboard input, 
then plugged controller again, the controller input will be forever lost. F6 serves as force re-connect hotkey if auto recognization upon re-plug fails. (Aceearly1993)    


#### [1.5.9] - 2025/6/15 #### 

`CHANGED` - Minor adjusts of in-game shop prices.    (Aceearly1993)  
`CHANGED` - The invincibility time of enemies against Holy Water is now 2 frames shorter than vanilla.  (Aceearly1993)  
`CHANGED` - Altar: The behavior of the heart recover zone to match the behavior of the same mechanic seen in prologue, 
for a better presentation approach.  (Aceearly1993)  
`CHANGED` - Leviathan: Changed color of post-hit flash effect to the same color as Lucifer's post-hit flash effect in order to reduce visual confusions.  (Aceearly1993)  
`CHANGED` - Pause menu/Boss Rush/Endroll: Adjustments of mugshot graphics for a better presentation approach.  (Lee Russell /rinth444)  
`CHANGED` - Properties of Holy Water so that it can reach following enemies:  
Hanged  
Possessed Tree  
Upended Demon  
Count La Tourvelle  
Corpse Guest  
Duke Guillecourt (black hole)  
Lucifer  
 (Aceearly1993)  

`ADDED` - Alucard Player ("main Alcarde visible") : Straight upward jump animation.  (Lee Russell /rinth444)  
`ADDED` - Efrain player ("main hero visible") : Falling stance is now animated instead of a single graphic.  (Lee Russell /rinth444)  
`ADDED` - Update of endroll credit informations.  (Aceearly1993)  
`FIXED` - Trianon: A vanilla graphical error which a black tile was missing and left unnoticed until JupiterClimb's livestreams.  (Aceearly1993)  
`FIXED` - Dark Forest: One instance of Japanese text to be identical to other languages.  (Aceearly1993)  


#### [1.5.8] - 2025/5/4 #### 

`FIXED` - A bug in the new control mapping system which will cause controller mapping to be lost if you ignored control config in the very first time booting the game, 
go straight to action scene, then perform pause/map button pressing.   (Aceearly1993)  
`FIXED` - An oversight in the reworked boss rush timer formula which will cause victory music of Alucard's boss rush result screen to be missing.  (Aceearly1993)  
`FIXED` - A vanilla bug which will cause normal backpack infinitely purchasable in extremely conditions. (Aceearly1993)  
`CHANGED` - Some details in readme because some informations on "alternate build method" are no longer accurate.  (Aceearly1993)  


#### [1.5.7] - 2025/4/17 #### 

`FIXED` - Delbasee City park: A bug which will cause the 1000 g reward of a mutated plant to vanish.   (Aceearly1993)  
`FIXED` - An oversight which prevented the situation of Spike Armor's properties against certain spikes to be identical to vanilla.   (Aceearly1993)  
`FIXED` - A bug which will cause Efrain's movement stuck at the right wall of final boss room after a slide.  (Aceearly1993)  
`FIXED` - Gabrielle de La Tourvelle: A bug which will cause the Nine Gate book to vanish forever 
if you (somehow) leave the room without picking the Nine Gate book she offered (by utilizing out of bound glitch at left wall of Gabrielle's room).   (Aceearly1993)  
`CHANGED` - Delbasee City park: Position of movement box of a mutated plant's head to prevent overlapping with the wall's collision on its back,
disabling the possibilities of the 1000 g reward clipping into the wall.  (Aceearly1993)  
`CHANGED` - Gabrielle de La Tourvelle: Minor adjust to the order of her dialogue in order to fit the situation of the above fix.    (Aceearly1993)  
`CHANGED` - Rivoire Cave: Very slightly tweaked position of several backgrounds in order to not make them too overlapped.  (Aceearly1993)  
`CHANGED` - Guernon University: Very slightly edited the neutral graphic of a breakable wall in order to prevent explore progression problems.   (Aceearly1993)  
`ADDED` - Event editor: More notations of event related to enemy structure.   (Aceearly1993)  
`ADDED` - Important notes on Readme (Simplified Chinese) to counter Chinese-specific crash issues.   (Aceearly1993)  



#### [1.5.6] - 2025/2/28 #### 

`EXPERIMENT` - Changed Skeleton Gunman's behavior so that his bullet will now be a physical object instead of the bullet instantly reaches you as soon as he fires his gun.   
This change will have side effects so that the properties of his shots will no longer be identical to vanilla.   (Aceearly1993)  
`ADDED` - Arrow notations on a statue at Guernon University when the mechanism inside the statue is pulled down.   (Aceearly1993)  
`ADDED` - Instructions if you encountered crash exits for wrong reasons.  (Aceearly1993)  
`ADDED` - Ability to remember the window size set in video setting screen.  (Aceearly1993)  
`ADDED` - keyboard prompt notations in most of the remaining screens to let keyboard player not lost too quick.  (Aceearly1993)  
`FIXED` -  Servigny mansion's crypt: A bug which the size of one minimap mapchip object is incorrect.  (Aceearly1993)  
`FIXED` -  A bug which will cause the game to crash exit if unplug and replug the controller, then reset the game.  (Aceearly1993)  
`FIXED` -  An attempt to fix a irregular, bug-like phenomenon which the knockback animation will be incorrect if try to step on stairs while very close to an airbone enemy who's sticking to the air.  (Aceearly1993)  
`FIXED` -  A bug which keyboard input of Aura blast and Special action keys might be incorrect after entering control config through controller,
but changes keyboard keys and exits to action scene as keyboard.  (Aceearly1993)  
`FIXED` -  La Tourvelle Castle: An out of bound glitch which can be easily triggered and can cause progression problems. (Aceearly1993)  
`CHANGED` - Reorganized size of ending/credit roll text strings to make text size not too big (DX9 only).  (Aceearly1993)  
`CHANGED` - Global Event editor: Reorganized platform/stair events to be in groups more visible.  (Aceearly1993)  
`CHANGED` - Now you can carry 2 more High potions at once compared to vanilla.  (Aceearly1993)  


#### [1.5.5] - 2025/1/10 #### 

`CHANGED` - The logic of control config screen; The joypad remap and keyboard remap functions can be individually selected instead of cramming everything into the same config screen.     (Aceearly1993)  
`ADDED` - Important elements to reflect the changes of control config.     (Aceearly1993)  
`ADDED` - Alcuard boss rush: Collision physic correction when you're performing walk/slide on a Downhill slope, eliminated a bug-like behavior that you'll frequently switch between walk and fall states if walking downhill at full speed.    (Aceearly1993)  
`FIXED` - Underground Aqueduct: An out of bound bug which can happen if you strike a breakable wall while sticking very close to the breakable wall in question.    (Aceearly1993)  
`FIXED` - Underground Aqueduct: A irregular phenomenon so that the variable for the situation of a breakable wall is destroyed or not, will now be properly recorded.     (Aceearly1993)  



#### [1.5.4] - 2024/10/1 #### 

`ADDED` - Arrow notations of new texts at La Tourvelle's castle.    (Aceearly1993)  
`ADDED` - Arrow notations at save spots, warp spots, area transition room in Castle of Eternal night.    (Aceearly1993)  
`ADDED` - Arrow notations on all road signs at village and earldoms.     (Aceearly1993)  
`ADDED` - Arrow notations at top of ferryman's position when ferryman is prepared to bring you across the lake.     (Aceearly1993)  
`ADDED` - More event notations in the project file.    (Aceearly1993)  
`ADDED` - Arrow notations on a hint of a puzzle at Servigny Mansion.     (Aceearly1993)  
`ADDED` - Simplified Chinese counterpart of "owned" embedded text in shops.    (Aceearly1993)  
`ADDED` - Auto save function upon reach all possible endings in order to let player not lose too much progress by meeting undesired endings.    (Aceearly1993)  
`FIXED` - A softlock bug in game over> continue mechanic if you let the save slot keep empty on purpose by triggering an auto saving when you let Efrain reached the first town in the game.     (Aceearly1993)  
`FIXED` - A bug in the new auto save mechanic after final boss where you might be trapped at final boss room after beaten final boss before.  (Aceearly1993)  
`FIXED` - Remaining instances where you may get softlocked by dying through poison while Efrain is acrossing area transitions zones in the process.     (Aceearly1993)  
`CHANGED` - Now if the stone hand had been used in front of Count Servigny's courtyard, the arrow notation will correctly disappear.     (Aceearly1993)  
`CHANGED` - Organized the events of item sellers/vending machines into isolated groups for better visibility of any potential future editors.     (Aceearly1993)  
`CHANGED` - Enhancements of Garden of the Dead A-letter panel blink effect due to requests.     (Aceearly1993)  


#### [1.5.3] - 2024/9/14 #### 

`ADDED` - Availability of changing and saving controller labels (XBOX/D-input/PS).    (Aceearly1993)  
`ADDED` - Availability of mapping function keys to joypad's 11th and 12th buttons.    (Aceearly1993)  
`ADDED` - Availability of exiting the game without involving of mouse input.     (Aceearly1993)  
`ADDED` - Availability of saving the current situation of anti-aliasing settings.     (Aceearly1993)  
`ADDED` - Availability of function key inputs through xbox trigger buttons.     (Aceearly1993)  
`FIXED` - One instance at equipment screen that will cause confusions on Switch controller.     (Aceearly1993)  
`CHANGED` - The term "DEFAULT CONTROLS" to "CONTROL CONFIG" in control setting screen.     (Aceearly1993)  
`CHANGED` - Priority of attack event in the [move up/down on rope>attack] event string to be roughly the same as Christopher's in Belmont's Revenge.     (Aceearly1993)  
`CHANGED` - Now you can cancel the delay after a sword swing while crouching (by holding left or right), roughly resembles 
the properties in Alucard's crouching attack priority in Symphony of the Night.     (Aceearly1993)  


#### [1.5.2] - 2024/8/8 #### 

`CHANGED` - Eliminated the strange vanilla design choice that system hotkeys had used up "Space" keys; More user friendly for Players whose personal preferences are getting used to assign jump to "Space" key.    (Aceearly1993)  
`CHANGED` -Alucard player: Eliminated the additional knockback if taken damage while doing air dash in order to avoid confusions.    (Aceearly1993)  
`CHANGED` - UI logic to fit the tweaks of Control Config function in title menu and system config screens.    (Aceearly1993)  
`FIXED` - An attempt to fix the question marks at enemy bestiary being bugged in rare circumstances.   (Aceearly1993)  
`FIXED` - Video option 960p and 1080p indicator not working on keyboard.    (Aceearly1993)  
`ADDED` - Disclaimer screen back from demo version.    (Aceearly1993)  


#### [1.5.1] - 2024/8/2 #### 


`ADDED` - Music player function hidden somewhere in the game.  (Aceearly1993)  
`ADDED` - More event notations in the event groups.  (Aceearly1993)  


#### [1.5.0] - 2024/7/26 #### 


`CHANGED` - Position of Enemy bestiary HP/ATK/DEF texts (to match the quality in Chronicles of the Wolf).  (Aceearly1993)  
`CHANGED` - Update the enemy bestiary text format so that the rare item text will be obscured by darker color scheme if the item in question is yet to be collected. 
This is done to better visualize if the rare enemy item drop is collected or not. (Aceearly1993)  
`ADDED` - Function to remember if the game is set in full screen mode or windowed mode (to match the quality in Chronicles of the Wolf). (Aceearly1993)  
`ADDED` - Function to remember your boss rush best time (the same as LC1). (Aceearly1993)  
`ADDED` - Copies of event controller objects in order to memorize if the rare enemy drop equipment is collected or not in enemy bestiary. (Aceearly1993)  
`ADDED` - Indicator of Ring of fury mode label to indicate if you're on Ring of Fury mode or not. (Aceearly1993)  
`FIXED` - A vanilla bug which the attack power indicator of V.V. sword did not get instantly updated in the equipment menu. (Aceearly1993)  
`FIXED` - Trianon: A vanilla bug which one of the pick up item ID will be duplicated to another pick up ID. (Aceearly1993)  


#### [1.4.9] - 2024/6/28 #### 

`CHANGED` - Update the item pickup display text format so that text is no longer bugged in several mileseconds before acrossing the action scene transition zones 
while the pickup textbox is still active.  (Aceearly1993)  
`CHANGED` - Reworked Alucard air dash animation. (ACC (a.k.a."得枫.德广"))  
`FIXED` - Bugged behavior in puppet theater event that can lead to permanently losing Anna V.V. entry in enemy bestiary unless manually edit enemy bestiary region in save file.  
`FIXED` - A vanilla bug which will cause softlocks upon knocked to area transition through dying.  (Aceearly1993)  
`FIXED` - Incorrect information on mini map before actually explored the area in question.  (Aceearly1993)  
`ADDED` - Copies of some enemies that can be triggered after beating a certain boss, get rid of the situation 
that can lead to permanently losing entry of these enemies in enemy bestiary unless manually edit enemy bestiary region in save file.  (Aceearly1993)  




#### [1.4.8] - 2024/5/3 #### 

`CHANGED` - Logic of cursor speed in music box/monster bestiary menus so that they're easier to navigate.  (Aceearly1993)  
`CHANGED` - Logic of return function in title screen/system config so the return key won't get overlapped with confirm key in extreme conditions.  (Aceearly1993)  
`CHANGED` - UI elements to reflect the changes in title screen/system config.  (Aceearly1993)  
`CHANGED` - Logic of return function in pause menu/map screen to match the quality in Chronicles of the Wolf.  (Aceearly1993)  


#### [1.4.7] - 2024/4/17 #### 

`CHANGED` - Update the item pickup display text format so that text is no longer bugged in CHS/JPN after changing language via system config in the midst of item pickup display time period.
  (Aceearly1993)  
`CHANGED` - Update the action stage text format so that text is no longer bugged in CHS/JPN after changing language via system config in the midst of stage exploring.
  (Aceearly1993)  
`CHANGED` - Minor adjusts to fit the changed text format after implementing system config.  (Aceearly1993)  

#### [1.4.6] - 2024/3/29 #### 

`ADDED` - A copy of title option menu to pause mnu so that players won't have to lose current progress in order to change system settings like control remap and language.  (Aceearly1993)  
`CHANGED` - Speed of some actions in the actual title option menu screen to reflect the customizations done to the copied option menu inside pause menu.  (Aceearly1993)  
`CHANGED` - Customizations to config saving mechanic to fit the new config screen.  (DragonX24)  

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
- Lee Russell (rinth444) - animation enhancement
... and all the people in game credits.
