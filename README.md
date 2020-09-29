# VRNeoIKFKTool

This mod is one improving existing StudioNEOVR.dll which controls objects / IKFK markers on VR.  
This functions on VR controllers are as below,

- Grab objects / IKFK markers and move/rotation them
- Scale objects
- Call objects
- Parent objects /IKFK markers with own controllers

## [Installation]
1. Extract the zip file into User's HoneySelect directory.
2. Run your Game execution file with "--vr" option. 
3. Enjoy new functions on VR!

**Caution!** 
- This mod might rewrite some existing files and cause some bugs depending on User's environment.
  Please back up Game root folder before installing necessarily.
- I dont know you can or cant use this mod on StudioNeo. But if you use improved HoneySelect VRmod (one integrating IBL&LRE made by arthurOmanko), you would be able to use this mod on StudioNeo.  
- If you using other VR tools as of now except for here, your game might work unproperly. Then reconsider removing other VR tools (${GameFolder}/Plugins/*.dll files etc.).  

## [Requirements]
- Game updated with the last patch and DLC installed.
- Installed and set up SteamVR.
- public HoneySelect VRmod (by Eusth) or improved HoneySelect VRmod (one integrating IBL&LRE made by arthurOmanko). 

## [Mod Settings]
- Setting:      
  -- None

## [Modes & Controls]

## Tools

These tools are mainly meant to be used in *standing mode* but some of them are also available in *seated mode*. In order to use added new function, press the *menu button* on your VR controller. [See here an overview of buttons](https://forums.unrealengine.com/attachment.php?attachmentid=87367&d=1460020388).

**You can get in-game help any time by holding the menu button!**

### NeoIKFKTool (seated / standing)
![icon_gripmove_forGit](https://user-images.githubusercontent.com/68005887/94588610-176d9a00-02bf-11eb-98c2-c065f4624709.png)

- red marker : grabbing any object or IKFK marker  
- white marker : grabbing nothing but might select any marker  

#### UI/UX abstract on KoumeiTool
Tag      |  Move   | 
----     | ------  | 
only one hand needed
<kbd>menu</kbd>+<kbd>holding</kbd> | display function of each button
<kbd>trigger</kbd>+<kbd>moving</kbd> | grab objects / IKFK markers on markers
<kbd>trackpad</kbd> | select a marker
<kbd>trackpad</kbd>+<kbd>doubleClicks</kbd> | deselect selected marker
<kbd>grip</kbd>+<kbd>moving</kbd> | move and rotate myself
<kbd>trigger</kbd>+<kbd>doubleClicks</kbd> | grab selected object on GUI window
<kbd>trackpad</kbd> | select multi objects on GUI window
two hands needed
<kbd>trackpad</kbd>+<kbd>trackpad</kbd> | scale selected object (All-axis)
<kbd>trackpad</kbd>+<kbd>trigger</kbd> | scale selected object (each XYZ-axis)

## Settings & Tweaks
