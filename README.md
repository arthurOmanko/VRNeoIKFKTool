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
--None

## [Modes & Controls]

## Tools

These tools are mainly meant to be used in *standing mode* but some of them are also available in *seated mode*. In order to use added new function, press the *menu button* on your VR controller. [See here an overview of buttons](https://forums.unrealengine.com/attachment.php?attachmentid=87367&d=1460020388).

**You can get in-game help any time by holding the menu button!**

### KoumeiTool (seated / standing)
![preview](https://user-images.githubusercontent.com/68005887/92324350-d72e4980-f07b-11ea-9ac0-073b22da5fe8.png)

#### UI/UX abstract on KoumeiTool
Tag      |  Move   | 
----     | ------  | 
only one hand needed
<kbd>menu</kbd>+<kbd>holding</kbd> | display function of each button
<kbd>trigger</kbd>+<kbd>doubleClicks</kbd> | Koumei Wind (generates wind)
<kbd>trigger</kbd>+<kbd>holding + moving</kbd> | Koumei Strip (strips cloth of female in front of you.)
<kbd>grip</kbd>+<kbd>doubleClicks</kbd> | Koumei Gaze1 (along your sight, chara changes clothes)
<kbd>grip</kbd>+<kbd>holding + moving</kbd> | Koumei Grab/Touch (grabs and touches breasts, hips, hairs, skirts or items with DynamicBones etc.). This functions can also be used on other Tools.
<kbd>trackpad</kbd>+<kbd>doubleClicks</kbd> | Koumei Gaze2 (along your sight, chara changes accessories)
<kbd>trackpad</kbd>+<kbd>holding + moving</kbd> | Koumei Move (move + rotate)

### ChageLightColorTool (Standing / Seated)
![lightColor](https://user-images.githubusercontent.com/68005887/92324643-a996cf80-f07e-11ea-9c67-c6039d60e73d.png)

#### UI/UX abstract on ChangeLightColor
Tag      |  Move   | 
----     | ------  | 
only one hand needed
<kbd>trackpad</kbd>+<kbd>holding + moving</kbd> | Change intensity or colors of front directional light
<kbd>trigger holding</kbd>+<kbd>trackpad</kbd>+<kbd>holding + moving</kbd> | Change intensity or colors of back directional light
<kbd>menu</kbd>+<kbd>holding</kbd> | display each fuction

## Settings & Tweaks

Settings can be changed in the file *VRKoumeiToolConfig.xml*, which is generated the first time you start the game.  
Tag      | Default | Effect |
----     | ------  | ------ |
`<HandScale>` | 1,1,1 | The size of VR controllers.
`<VelocityBufferSize>` | 5 | The buffer for speed calculation of VR controllers. Bigger, more proper.
`<Damping>` | 0.2 | The inverse of speed of return from bones changing. Smaller, more speedy.
`<GrabDampingDivisor>` | 16 | The speed of return from bones changing when grabbing. Bigger, more speedy.
`<GrabForceMultiplikator>` | 8 | The strength of grabbing. Bigger, stronger.
`<TouchRadius>` | 0.1 | The effective range of touching.
`<GrabRadius>` | 0.15 | The effective range of grabbing.
`<FixVrLightning>` | true | Whether or not using Light Color Tool on VR.
`<PleasureForceMin>` | 0.1 | The minimum of strength of grabbing for going finishing.
`<BreastPleasure>` | 0.0005 | The rate of increasing of pleasure on grabbing. On breasts or hips, effective.
`<WindStrength>` | 1 | The strength of wind.
`<WindDuration>` | 0.8 | The duration of wind. Bigger, more duration. [0 .. 0.999]
`<StripForce>` | 0.005 | The needed speed of VR controllers for stripping cloth.
`<StripRadius>` | 0.15 | The maximum of needed range for stripping cloth.
`<HasRumbling>` | true | Whether or not rumbling when touching. 'Rumble = true' setting needed in VRGIN Setting.
`<RumbleRadius>` | 0.07 | The effective range of rumbling when touching.
 
