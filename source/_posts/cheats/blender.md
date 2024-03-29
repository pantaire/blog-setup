---
title: Cheat Sheet - Blender
date: 2021-05-05 22:56:33
category: cheatsheet
tags:
    - blender
    - cheatsheet
    - art
    - modeling
excerpt: Navigate Blender easily
cover: ''
---

### Last Updated: 03.07.2021

# Cheatsheet for Blender Hotkeys

[RC] = right click  
[LC] = left click   
[MM] = middle mouse button (scrolling wheel)  


# Access Menus  
| [Shift] + [A] 	|            open add menu (object mode only)            	|
|-------------	    |------------------------------------------------------ 	|
| [Z]           	| open solid/wireframe/... menu                          	| 
| [Shift] + [S] 	| open cursor pie menu                                   	| 
| [F3]          	| open search menu                                       	|
| [N]           	| open property menu (menu on the right)                   	|  
| [~]           	| open pie menu for viewport (also accesible via numpad) 	|   
| [A]           	| open mask menu (in Sculpt Mode)	                        |   


# Selecting  
| [A]          | Select everything / whole object                                       |
|--------------|------------------------------------------------------------------------|
| [C]          | Select circle (rightclick to select, middle mouse button to de-select) |
| [Alt] + [LC] | Select loop                                                            |
| [Ctrl] + [I] | Invert Selection                                                       |
| [H]          | Hide selected object                                                   |
| [Alt] + [H]  | Show hidden object                                                     |
| [Alt] + [LC] | Select ring/loop                                                       |


# Object Manipulation  
| Shortcut           | Command                                                                                                  |
|--------------------|----------------------------------------------------------------------------------------------------------|
| [Tab]              | Switch between last used modes (e.g. edit/object mode)                                                   |
| [Shift] + [Z]      | Switch between last used views (e.g. wireframe/solid/rendered)                                           |
| [Shift] + [D]      | Duplicate object                                                                                         |
| [Shift] + [R]      | Add middle vertex, subdivide vertices                                                                    |
| [Ctrl] + [1-4]     | Add Subdivision Modifier with 1-4 Subdiv depth                                                           |
| [Ctrl] + [A]       | Morph around vertex (like Scale [S]), useful when sculpting and brush is stretched (must be object mode) |
| [Esc] / [RC]       | Snap back to last position                                                                               |
| [S] + [Axis] [-1]  | Mirror object on [Axis]                                                                                  |
| [S] + [Axis] [0]   | Align object on [Axis]                                                                                   |
| [F]                | Fill distance (hook points must be selected)                                                             |
| [Ctrl] + [Num]     | Add [Num] amount of subdivisions                                                                         |
| [G]                | grab active object                                                                                       |
| [R]                | rotate active object                                                                                     |
| [S]                | scale active object                                                                                      |
| [E]                | Extrude (drag part of the object)                                                                        |
| [X]                | delete active object                                                                                     |
| [Shift] + [R]      | drag mouse to change voxel resolution (kinda like dyntopo, but cool)                                     |  


# Vertices  
| Shortcut          | Command                                  |
|-------------------|------------------------------------------|
| [Alt] + [M]       | Merge Vertices (must be in edit mode)    |
| [K]               | Knife (cut vertex)                       |
| [K] + [Z]         | Cut along midline of connecting vertices |
| [K] + [Alt]       | Change number of cutting points          |
| [S] + [Z] + [0]   | Flatten selected points along z axis     |


# Viewport/Camera  
| Shortcut         | Command                                                                  |
|------------------|--------------------------------------------------------------------------|
| drag corner      | add window (split view)                                                  |
| [Numpad 1-9]     | Navigate viewport                                                        |
| [Numpad 0]       | snap in/out of camera viewpoint                                          |
| [Shift] + [F]    | Fly camera (navigate with W,A,S,D) ?                                     |
| [R/G] + [X/Y/Z]  | Move camera along world axis, press axis twice to move along camera axis |
| [Alt] + [MM]     | Drag to snap to next axis, click to set view center to mouse position    |
| [Ctrl] + [MM]    | Move up/down to zoom                                                     |
| [Shift] + [MM]   | Drag View                                                                |
| [Ctrl] + [Space] | Toggle Full Screen on active window                                      |
| [MM]             | Drag viewpoint, click to jump to view (object mode only)                 | 


# Cursor
| Shortcut       | Command                                               |
|----------------|-------------------------------------------------------|
| [Shift] + [RC] | move cursor (the point where new objects are created) |
| [Shift] + [C]  | move cursor to center ( coordinates: 0,0,0)           |
| [Shift] + [S]  | open cursor pie menu                                  |


# Modifiers
Always apply from top down, and don't forget to apply!  


## Boolean  
| Setting    | What it does                                                                                                                          |
|------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Intersect  | takes the two objects and keeps only the volume that they both occupy, removing everything else                                       |
| Union      | takes both objects and tries to fuse them together where they intersect, adding the volumes together and create one object            |
| Difference | takes one object and cuts out the volume that it shares with another object, “cutting” into it based on the shape of the first object |


# Edit Mode
[Ctrl] + [N] (+[Shift]) Recalculate Normals


# Simulation
Cache: bring to replay to get a first overview over the simulation  
Apply changes/empty cache: Click on a setting and hit enter, cache is emptied automatically  
Bake: Set from [replay] to [modular], bake Fluid first  
move down the line and bake mesh, particles,... (must be checked to be effective)  


# Sculpting
Hotkeys are visible on hover
If brush seems to be not round, apply scale in Object mode  
Masks are your friend, use them

| Shortcut | Command                                                                 |
|----------|-------------------------------------------------------------------------|
| [F]      | Resize Brush                                                            |
| [Ctrl]   | Change Brush Direction (subtract/add), must stay pressed to take effect |
| [X]      | Draw Mode                                                               |
| [C]      | Clay Mode                                                               |
| [G]      | Grab Mode                                                               | 


# Merging stuff  
[Ctrl] + [J]            Join Objects  
Sculptmode -> Remesh    to delete inner faces and get quads (but kindof destroys topology)  
[Ctrl] + [Shift] + [B]  join meshes, booltool must be enabled (Edit -> Preferences -> Booltool)  
                            - union: delete inner mesh  
                            - intersect: only keep middle  


# UV / Texture Paint
Edit Mode, select Everyting [A]  
[U] -> Smart Unwrap, may take a few secs  
Workspace: Add texture based on roughness, metallic, base colour, ...  
start drawing  
[S] sample colour  


# Curves
Array Modifier to curve: Add Array mod to object, generate a curve. Add curve mod to object, pick curve as origin. Adjust array object count on object to fit the curve  

# Rigging
Add Human rig with rigify (comes pre-installed, but needs to be activated)  
Scale to model, apply scale in Object Properties (Ctrl + A -> Apply all transforms)  
Rigging Tab: Click generate rig  
Select all model parts, then select rig last, hit Ctrl + P -> Set parent with automatic weights  
Switch to Pose Mode to move things around   
Press N for more options, e.g. Not making limbs stretch when moving the handle too much  

# 2D Animation / Grease Pencil
| Shortcut              | Command                                                                                     |
|-----------------------|---------------------------------------------------------------------------------------------|
| [Shift] + [F]         | change strength (as opposed to radius with F)                                               |
| [U]                   | change active normal material                                                               |
| [Y]                   | change active layer                                                                         |
| [I]                   | insert frame                                                                                |
| [H]                   | hide active layer                                                                           |
| [Shift] + [H]         | hide inactive layers                                                                        |
| [Alt] + [H]           | unhide everything                                                                           |
| [Alt]                 | hold down to draw straight horizontal/vertical lines                                        |
| [Shift]               | draw straight lines                                                                         |
| [Shift] + [Alt]       | draw straight lines, but extend on both sides when drawing. works for circles and boxes too |
| [Ctrl]                | hold down to erase                                                                          |
| [Ctrl] + [Alt]        | hold down for lasso tool to loop erase                                                      |
| [Alt] + [S]           | Change Stroke radius                                                                        |
| [L]                   | Select linked                                                                               |
| [Shift] + [G]         | Select grouped                                                                              |
| [Ctrl] + [Numpad +/-] | Select more/less points                                                                     |


# Timelines
use normal modification (g, s, e, ...) to modify timeline and keyframes  

| Shortcut      | Command            |
|---------------|--------------------|
| [B]           | Box Select         |
| [C]           | Circle Select      |
| [Shift] + [R] | Repeat last action |


# Retopo Hacks
Mouth corners: J to split, Subdivide to redirect upper lip loop to lower lip loop (instead of down to chin)
Never have 3 or 5 connection vertices on a crease. Instead, insert a clean line for the crease and move the 3s or 5s out-/inwards.


# Edit Texture in Krita
Prerequisites: Preferences > File Paths > Applications > Image Editor > set to Krita.exe location  
Add Material and Image Texture to Object (Shader Menu)  
Tab into Texture Paint Mode, open side (N) menu, navigate to Tool > Options > External  
Set Screen Grab size, choose Quick Edit, wait for Krita to open  
Make changes, save, go back to Blender, click Apply in same menu


# Geometry Nodes  
Point Instance      adds a point on every vertex


# Vocabs  
Dyntopo         adds/removes details on the fly, regular sculpting only affects shape of mesh  
Upres factor    adds details to simulations  

# Addons / Useful Software
| Name                  | what it do                       |
|-----------------------|----------------------------------|
| BY-GEN                | generates stuff                  |
| Bsurfaces GPL Edition | idk                              |
| Animation Nodes       | idk                              |
| Bool Tool             | boolean stuff                    |
| Rigify                | rigs stuff                       |
| fSpy                  | find focal center & align lines  |
| MakeHuman             | generates humanoids like in GTA  |
| PureRef               | arrange and collect reference    |
