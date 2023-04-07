## Description
Source code of the fan-game Castlevania: The Lecarde Chronicles 2 made by Migami Games. Due to a HDD failure, the original source have been lost. This repo is an atempt to preserve, fix and improve this game.

Unfortunately, the recovery process ended up corrupting all non-English characters, many transparency effects and more. So, if you know any of the following languages and is interested in helping us out by fixing and re-translating this project, feel free to contact us, we are in need of:
- ~~French~~ Since Mig himself is the French translator, French translation *technically* should be accurate enough.
- Spanish
- German
- ~~Italian~~ Jeffrey Montoya says the Italian translator usually worked for every Migami Games project, So it's...fine to keep the original script until there're some critical Italian translation error spotted.
- ~~Japanese~~ Initial Japanese translation script found! (thanks: theplottwist)
- ~~Brazilian Portuguese~~ Initial Brazilian Translation script found! (thanks: theplottwist)

## Disclaimer
We contacted Migami Games and got approval to keep this repository up.  

The release of Lecarde Chronicles 2 got permited by Konami, the game and its assets are freeware and **_SHOULD NOT_** be sold, this also includes the source code. Any modifications you do have also to be free. Castlevania is an intelectual property owned by Konami, please support the company by buying their official releases. 

## Usage
To get the reworked game builds, go to "Releases", choose the latest "v*. *. *-alpha" tag and find the .exe file. The .exe file is the generated executable, while the .mfa file is the (recovered) Clickteam Fusion project file necessary to generate the .exe (note in this game's case, it requires some extensions from Clickteam Fusion 2.5 Developer builds to be opened). 

Note that the original game is infamous for the compatibility for controllers if your computers are unlucky so it left the controller preference blank. Here's a valid workaround to this issue if you encountered it like me:

In Control Panel→ Devices and printers, find PS4 controller (usually labeled as "Wireless Controller"), right click "Wireless Controller" label to find controller setting, then click "advance..." to go into advance setting of "Wireless Controller", and be sure the "Wireless Controller" is checked as the preference.

The same could be applied to Xbox Controllers by repeating the setup above while your desired Xbox controller is plugged in.

## Changelog

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
