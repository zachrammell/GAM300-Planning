### Game:
Game needs to be fast paced and full of action  
Sekiro/Infinity Blade/For Honor style sword combat  
Racing Game - can jump to other racers and duel them with swords  
take control of their cars(?)  
Shrek smash and crash  
potentially more linear idea with 1v1 races switching from racing to fighting and back again  
Rendering - PBR? More stylized? Global Illumination? Will need to cut corners somewhere. Also highly dependent on art style  

### Team Culture:
Team should be fun to work with, people shouldn't feel left out  
We will have distinct times for working and hanging out to stay productive but also have fun  
We are all equals, titles mean nothing, only responsibilities and work done.  
Never be afraid to bring up your own ideas, or to challenge existing ones  

### Programming:
Make the engine for the game, not a generic thing. A engine feature should not be added if it doesn't directly support a game feature.
Favor simple and extensible code over perfectly architected and generic code.

When writing code:
- Make it compile
- Make it run and get the right output
- Make it fast

No "Code Ownership," you are free to change other people's code.
However, all code will be reviewed, and if you edit someone else's code they should review it.

### Engine Architecture Ideas:
Data Oriented ECS
No RTTI or Exceptions
Live Update C++
Libraries to use:
EASTL, DirectXMath, GLFW(Win32 only if it doesn't work), Dear IMGUI, magic enum, 
A simple editor with Unity style object manipulation, component editing, Debug camera window
Multithreading only on specific systems as needed (i.e. physics) - use a thread pool
Level Folders with one file per object in the level
Things to consider:
Flatbuffers

### Tools we want to use:
Version Control - Git  
Build System - CMake  
IDE - Visual Studio or CLion  
3D Modeling - Blender (or Maya if available)  
Model Format - glTF  
Graphics API - DX11 (other APIs only for if we support other platforms)  

Targeting Windows 64 bit (other platforms only if we have time)

### Stuff to figure out:
Something to manage binary assets without putting them in git submodule
