# VRNeoIKFKTool

This mod is one improving existing StudioNEOVR.dll which controls objects / IKFK markers on VR.  
This functions on VR controllers are as below,

- Grab objects / IKFK markers and move/rotation them
- Operate IK/FK weight
- IK/FK shown or not shown
- Scale objects
- Call objects in front of you
- Parent objects / IKFK markers with own controllers (syncing both)
- Make VRCamera follow Game MainCamera or any selected gameObject
- Move and Rotate

## [Installation]
1. Extract the zip file into User's HoneySelect directory.
2. Run your Game execution file with "--vr" option. 
3. Enjoy new functions on VR!

**Caution!** 
- This mod might rewrite some existing files and cause some bugs depending on User's environment.
  Please back up Game root folder before installing necessarily.
- I dont know you can or cant use this mod on StudioNeo. But if you use improved HoneySelect VRmod (one integrating IBL&LRE made by arthurOmanko), you would be able to use this mod on StudioNeo.
- GGmod DLL (for clothes with high heels) might sometimes affect IK/FK of chara with high heels attached by GGmod, so during VR environment, the look, necklock, leap motion up to a chara or IK/FK of the chara might sometimes get weird. Then once please take off/put on clothes (especially high heels attached by GGmod). The any weird situation of the chara would get fixed.
- If you using other VR tools as of now except for here, your game might work unproperly. Then reconsider removing other VR tools (${GameFolder}/Plugins/*.dll files etc.). For example, might have to remove StudioNEOVR.dll, GripMoveForHSVRStudio.dll or GripMoveForHSVR.dll.  

## [Requirements]
- Game updated with the last patch and DLC installed.
- Installed and set up SteamVR.
- public HoneySelect VRmod (by Eusth) or improved HoneySelect VRmod (one integrating IBL&LRE made by arthurOmanko).
- HSStudioNEOAddon.dll version 0.9.2 (or more (not guaranteed))
- ${GameFolder}\Plugins\0Harmony.dll

## [Uninstall]
Please remove VRNeoIKFKTool.dll in (${GameFolder}\Plugins).

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
Tag                |  Move     | 
:------------:     | ------  | 
only one hand needed
<kbd>menu</kbd>+<kbd>holding</kbd> | display function of each button and recenter GUI window (+ 2.0s)
<kbd>trigger</kbd>+<kbd>DoubleClicks</kbd> | select and grab selected object on GUI window
<kbd>trackpad</kbd> | select multiple objects on GUI window
<kbd>trigger</kbd>+<kbd>moving</kbd> | grab and move/rotate a object / IKFK marker on the object / marker (or already selected one). Or When 0% weight of the marker, the weight gets 100%.
<kbd>trigger</kbd>+<kbd>DoubleClicks</kbd> | change the value of a IKFK marker weight on the marker (100% -> 50% -> 0%) (only for markers of charas whose weights once were changed before by grip Triple/Quadruple clicks)
<kbd>trigger</kbd>+<kbd>DoubleClicks</kbd> | IKFK markers shown or not shown (when not on a object / IKFK marker, laser for GUI invisible)
<kbd>trackpad</kbd> | select a object / IKFK marker on the object / marker. User gets able to manipulate it from a distance.
<kbd>trackpad</kbd>+<kbd>DoubleClicks</kbd> | deselect selected object / IKFK marker and ungrab all grabbed one 
<kbd>grip</kbd>+<kbd>TripleClicks</kbd> | make weights of all IKFK markers (only enabled) of selected charas get 100%. During chara animation, IKFK positions fixed.
<kbd>grip</kbd>+<kbd>QuadrupleClicks</kbd> | make weights of all IKFK markers (only enabled) of selected charas get 0%. During chara animation, IKFK positions unfixed.
<kbd>grip</kbd>+<kbd>moving</kbd> | move and rotate myself
<kbd>grip</kbd>+<kbd>trigger</kbd>+<kbd>menu</kbd>+<kbd>0.5s</kbd> | All axes rotation on/off when moving
two hands needed
<kbd>1.trackpad</kbd>+<kbd>2.trackpad</kbd> | scale selected object (All-axis)
<kbd>1.trackpad</kbd>+<kbd>2.trigger</kbd> | scale selected object (each XYZ-axis along with controller)
## About manipulating the weight of IK/FK marker
Advanced IK from HSStudioNEOAddon.dll can manipulate weights of a chara's IK [0..1]. This mod enables to manipulate the weights for both IK/FK by VR controllers using it.
**This can be used in order to manipulate all or parts of selected charas without stopping animation during chara animation on VR environment.**  
User can select some charas on GUI (by trigger or trackpad push) and when grip + Triple/Quadruple clicks, all IK and some of all enabled FK markers of selected charas are registered within mod data and their weights get able to be controlled. 
(Caution: currently only FK markers of neck and hands can be registered within mod data. Other FK markers (toe (body), hairs, skirts etc.) can not be registerd so their weight not controlled by this mod. 
If User does not want FKs fixed during animation, disable the FKs from the game menu in advance).   
In case that IKFK weights set for selected charas by this mod (grip + Triple/Quadruple clicks), when weight of a IKFK marker is 0% (0.0), the marker moves with charas and does not fix any chara's moving at correspondent bone.
Or when weight of a IKFK marker is 100% (1.0), the marker fixes chara's moving at correspondent bone. When weight of a IK marker is 50% (0.5), the marker fixes, to some extent, chara's moving at correspondent bone.  
Weight of IKFK marker can be changed by (trigger + Double clicks) on the marker, 100% (-> 50% for only IK) -> 0%. Or When trigger 0% marker, weight of the marker gets 100%.
Especially when chaging weights of markers of arm or leg by (trigger or trigger + Double clicks on a marker), weights of both red and blue markers attached at it are changed to same value at same time.  
As I mentioned earlier, GGmod DLL (for clothes with high heels) might sometimes affect IK/FK of chara with high heels attached by GGmod, 
so during VR environment, the look, necklock, leap motion up to a chara or IK/FK of the chara might sometimes get weird. 
Then once please take off/put on clothes (especially high heels attached by GGmod). The any weird situation of the chara would get fixed.  
Advanced IK GUI can do same in more details on both VR and normal environment (on only IK not FK).  

<table>
<tr align="center">
  <th> </th>
  <th>Weight 100% (1.0)</th>
  <th>Weight 50% (0.5)</th>
  <th>Weight 0% (0.0)</th>
</tr>
<tr align="center">
  <th>IK (red)</th>
  <th><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/ebc447d1-5c18-4e92-b783-397ce70e7dcf" width="50" height="50"></th>
  <th><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/b18c94c4-f51b-4c1a-b6ae-fda228e0652f" width="50" height="50"></th>
  <th><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/b161b42d-1ad6-47aa-9964-29701a02d554" width="50" height="50"></th>
</tr>
<tr align="center">
  <td>IK (blue)</td>
  <td><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/1000aaab-5027-4c42-b27e-15bb1281decf" width="50" height="50"></td>
  <td><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/40b63852-56ef-4364-9a54-7143c02b1634" width="50" height="50"></td>
  <td><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/96458dd8-eb15-48b4-b61f-61627cfbce03" width="50" height="50"></td>
</tr>
<tr align="center">
  <td>FK (white)</td>
  <td><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/c32175c7-bd0f-4178-9538-cc55efe35347" width="50" height="50"></td>
  <td>---</td>
  <td><img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/ea8aa8f8-ab26-42b8-95dd-54a83e9dfc02" width="50" height="50"></td>
</tr>
</table>

## Option on GUI window
### Trigger each icon on GUI window  

![icon_call](https://user-images.githubusercontent.com/68005887/94591985-c7dd9d00-02c3-11eb-85b5-dbe3c541413c.png)

- Call a object in front of you

![icon_call_xz](https://user-images.githubusercontent.com/68005887/94592000-ca3ff700-02c3-11eb-802a-b275d15bfb65.png)

- Call a object in front of you (except for the height)

![parent_child](https://user-images.githubusercontent.com/68005887/94592023-cd3ae780-02c3-11eb-98c9-1e312babd3c2.png)

- Parent selected marker with your controller (object syncing with your controller moving/rotating)

<img src="https://github.com/arthurOmanko/VRNeoIKFKTool/assets/68005887/e818d50e-6ab9-420e-aeaa-15007ec047b8" width="200" height="150">

- [Advanced IK]: same as one from HSStudioNEOAddon.dll. User can manipulate details (weights etc.) of IK, AutoTrack for parent/child or start VMD (MikuMikuDance) etc. About MMD, by installing other appriciate mods, User might also be able to do same on VNGE.
- [Move with Main Camera]: VRCamera moves with Game Main Camera. For example, this enables VRCamera to emulate moving camera of MMD (MikuMikuDance). 
- [Move with Item]: VRCamera moves with selected GameObject. For example, this enables VRCamera to follow selected moving gameObject. 

