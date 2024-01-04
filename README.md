# VRNeoIKFKTool

This mod is one improving existing StudioNEOVR.dll which controls objects / IKFK markers on VR.  
This functions on VR controllers are as below,

- Grab objects / IKFK markers and move/rotation them
- Operate IK/FK weight
- Scale objects
- Call objects in front of you
- Parent objects / IKFK markers with own controllers (syncing both)
- Make VRCamera follow with Game MainCamera or any selected item
- Move and Rotate

## [Installation]
1. Extract the zip file into User's HoneySelect directory.
2. Run your Game execution file with "--vr" option. 
3. Enjoy new functions on VR!

**Caution!** 
- This mod might rewrite some existing files and cause some bugs depending on User's environment.
  Please back up Game root folder before installing necessarily.
- I dont know you can or cant use this mod on StudioNeo. But if you use improved HoneySelect VRmod (one integrating IBL&LRE made by arthurOmanko), you would be able to use this mod on StudioNeo.
- GGmod DLL (for clothes with high heels) might sometimes affect IK/FK of chara with high heels attached by GGmod, so during VR environment, the look, necklock or IK/FK of the chara might sometimes get weird. Then once please take off/put on clothes (especially high heels attached by GGmod). The any weird situation of the chara would get fixed.
- If you using other VR tools as of now except for here, your game might work unproperly. Then reconsider removing other VR tools (${GameFolder}/Plugins/*.dll files etc.). For example, might have to remove StudioNEOVR.dll, GripMoveForHSVRStudio.dll or GripMoveForHSVR.dll.  

## [Requirements]
- Game updated with the last patch and DLC installed.
- Installed and set up SteamVR.
- public HoneySelect VRmod (by Eusth) or improved HoneySelect VRmod (one integrating IBL&LRE made by arthurOmanko).
- StudioNEOAddon.dll ver

## [Mod Settings]
- Setting:      
  -- None

## [Modes & Controls]

## Tools

These tools are mainly meant to be used in *standing mode* but some of them are also available in *seated mode*. In order to use added new function, press the *menu button* on your VR controller. [See here an overview of buttons](https://forums.unrealengine.com/attachment.php?attachmentid=87367&d=1460020388).

**You can get in-game help any time by holding the menu button!**

### NeoIKFKTool (seated / standing)
![icon_gripmove_forGit](https://user-images.githubusercontent.com/68005887/94588610-176d9a00-02bf-11eb-98c2-c065f4624709.png)

- red marker : preparing to grab or select a object / IKFK marker, or already grabbing or selecting any object / IKFK marker  
- white marker : grabbing or selecting nothing  

#### UI/UX abstract on KoumeiTool
Tag      |  Move   | 
----     | ------  | 
only one hand needed
<kbd>menu</kbd>+<kbd>holding</kbd> | display function of each button and recenter GUI window
<kbd>trigger</kbd>+<kbd>DoubleClicks</kbd> | select and grab selected object on on GUI window
<kbd>trackpad</kbd> | select multi objects on GUI window
<kbd>trigger</kbd>+<kbd>moving</kbd> | grab a object / IKFK marker on the object / marker. Or if 0% weight of the marker, the weight gets 100%.
<kbd>trigger</kbd>+<kbd>DoubleClicks</kbd> | change the value of a IKFK marker weight on the marker (100% -> 50% -> 0%) (only for markers of charas whose weights once were changed before by grip Triple/Quadruple clicks)
<kbd>trigger</kbd>+<kbd>DoubleClicks</kbd> | IKFK markers shown or not shown (when not on a object / IKFK marker, laser for GUI invisible)
<kbd>trackpad</kbd> | select a object / IKFK marker on the object / marker. User can manipulate it from a distance.
<kbd>trackpad</kbd>+<kbd>DoubleClicks</kbd> | deselect selected object / IKFK marker and ungrab all grabbed one 
<kbd>grip</kbd>+<kbd>TripleClicks</kbd> | make weights of all IKFK markers (only enabled) of selected charas get 100%. During chara animation, IKFK positions fixed.
<kbd>grip</kbd>+<kbd>QuadrupleClicks</kbd> | make weights of all IKFK markers (only enabled) of selected charas get 0%. During chara animation, IKFK positions unfixed.
<kbd>grip</kbd>+<kbd>moving</kbd> | move and rotate myself
<kbd>grip</kbd>+<kbd>trigger</kbd>+<kbd>menu</kbd>+<kbd>0.5s</kbd> | All axes rotation on/off when moving
two hands needed
<kbd>trackpad</kbd>+<kbd>trackpad</kbd> | scale selected object (All-axis)
<kbd>trackpad</kbd>+<kbd>trigger</kbd> | scale selected object (selected each XYZ-axis)

## Option on GUI window
### Trigger each icon on GUI window  

![icon_call](https://user-images.githubusercontent.com/68005887/94591985-c7dd9d00-02c3-11eb-85b5-dbe3c541413c.png)

- Call a object in front of you

![icon_call_xz](https://user-images.githubusercontent.com/68005887/94592000-ca3ff700-02c3-11eb-802a-b275d15bfb65.png)

- Call a object in front of you (except for the height)

![parent_child](https://user-images.githubusercontent.com/68005887/94592023-cd3ae780-02c3-11eb-98c9-1e312babd3c2.png)

- Parent selected marker with your controller (object syncing with your controller moving/rotating) 
