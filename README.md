## Description
Source code of the fan-game Castlevania: The Lecarde Chronicles 2 made by Migami Games. Due to a HDD failure, the original source have been lost. This repo is an atempt to preserve, fix and improve this game.

Unfortunately, the recovery process ended up corrupting all non-English characters, many transparency effects and more. So, if you know any of the following languages and is interested in helping us out by fixing and re-translating this project, feel free to contact us, we are in need of:
- ~~French~~ Since Mig himself is the French translator, French translation *technically* should be accurate enough.
- Spanish: After discussions, we decided to keep the original state of Spanish text as much as possible for "Catoblepas" builds until there're some critical Spanish translation error spotted.
- German: Same as Spanish.
- Italian: Jeffrey Montoya says the Italian translator usually worked for every Migami Games project, So it's... fine to keep the original script in "Catoblepas" builds until there're some critical Italian translation error spotted.
- ~~Japanese~~ Initial Japanese translation script found! (thanks: theplottwist)
- ~~Brazilian Portuguese~~ Initial Brazilian Translation script found! (thanks: theplottwist)

## Disclaimer
We contacted Migami Games and got approval to keep this repository up.  

The release of Lecarde Chronicles 2 got permited by Konami, the game and its assets are freeware and **_SHOULD NOT_** be sold, this also includes the source code. Any modifications you do have also to be free. Castlevania is an intelectual property owned by Konami, please support the company by buying their official releases. 

## Usage
To get the reworked game builds, go to "Releases", choose the latest "v*. *. *-alpha" tag and find the .exe file. The .exe file is the generated executable, while the .mfa file is the (recovered) Clickteam Fusion project file necessary to generate the .exe (note in this game's case, it requires some extensions from Clickteam Fusion 2.5 Developer builds to be opened). 

Note that the original game is infamous for the compatibility issue for PS4/Xbox controllers if your computers are unlucky so it left the controller preference blank. Here's a valid workaround to this issue if you encountered it like us:

In Control Panel→ Devices and printers, find PS4 controller (usually labeled as "Wireless Controller"), right click "Wireless Controller" label to find controller setting, then click "advance..." to go into advance setting of "Wireless Controller", and be sure the "Wireless Controller" is checked as the preference.

The same could be applied to Xbox Controllers by repeating the setup above while your desired Xbox controller is plugged in.


## Changelog

#### [0.9.0.0] - 2023/6/5 #### 
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


#### [0.8.0.0] - 2023/6/1 #### 

`ADDED` - Missing counterparts of brazilian-portuguese texts and pictures. (Aceearly1993 & Katriel)  
`CHANGED` - Two instances in Japanese script for consistency of second personel. (Aceearly1993)  
`CHANGED` - Soft reset command from F2 key to Ctrl+F2 key to avoid accident misinput. (Aceearly1993)  
`CHANGED` - Description ("Guide") screen UI to reflect global function hotkey changes. (Aceearly1993)  
`FIXED` - Unique icon of plain text object for better visibility in frame editor. (Aceearly1993)  
`FIXED`  - An attempt to address issues with frame speed in Alucard player's walking animation. (Aceearly1993)  
`FIXED`  - Graphic error in the Alucard event animation in St. Justin. (Aceearly1993)  
`FIXED`  - Issues with consistency of distances between text at S.Chinese title menu. (Aceearly1993)  
`FIXED`  - Finalized and restored unused brazilian-portuguese variant of teleport room embedded texts. (Aceearly1993)  



#### [0.7.0.4] - 2023/5/28 #### 

`ADDED` - Recovered all brazilian-portuguese original dialogue, as well as fixed several issues and mistranslations.  
`FIX` - Wrong images on some shops.  
`FIX` - Brazilian-portuguese text alignment.  

#### [0.7.0.3] - 2023/5/17 #### 

`ADDED` - A task bar system which can be freely toggled on/off by pressing F8 key, previously only seen in an early demo of the game, and LC1.   

The option menu bundled within this task bar, has a built-in control option which can change the secondary variant of keyboard direction key mapping to anywhere else (There's no character stuck bug in the secondary keyboard direction key mapping), effectively countering the keyboard control bug as a temporary solution until we solved in-game control mapping bug in Mig's bottom-level code system in the future.    

#### [0.7.0.2] - 2023/5/16 #### 

`FIXED` - Small Keyboard region Control in save room.

#### [0.7.0.1] - 2023-05-16

`ADDED` - Small keyboard region control inspired from the original.  (Aceearly1993)  
`ADDED` - Extended Readme.  (Aceearly1993)  
`ADDED` - Japanese variant of "super load" screen area name text. (Aceearly1993)  
`CHANGED` - Reverted font of equipment name back to original. (Aceearly1993)  
`CHANGED` - Japanese and Simplified Chinese language variants now use unique font for equipment name. (Aceearly1993)  
`CHANGED` - One instance in S.Chinese script. (Aceearly1993)  



#### About Small keyboard region control #### 

 Small keyboard region control is inspired from the original keyboard control, added back by requests as the current keyboard rebind control has bugs.  
Keys are set below:  
- "Ins": Attack  
- "Del": Jump  
- "End": Special   
- "Page Down": Aura  
- "-": Map Screen  
- "+": Sub Menu  


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
- mashedpotatoes312
- theplottwist
- 狼王之2型 (https://space.bilibili.com/936194/dynamic) (Japanese re-translation)

... and all the people in game credits.
