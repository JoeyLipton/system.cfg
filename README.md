<h1 align="center">CryEngine system.cfg No Shadows</h1>

## How it works

Like every game engine, there is a console to type in commands to directly enable or disable certain aspects of the game. You'll find very often that a lot of settings that are available in the console do not have in-game UI representations. Now what if im making a game and need to run like 20 commands to enable developer tools, wireframe, visible hitboxes, etc.? That's what script files are for, these are essentially line-by-line text files that run as console commands.

CryEngine uses three location to locate a games configuration file:
1. %USER%/game.cfg
2. root/system.cfg
3. root/user.cfg

Most CryEngine games use one or more of these files depending on the structure. For example, a multiplayer game that requires authentication might store your settings client-side in the `%USER%/game.cfg` and not use any other files. The only issue is that developers might not bother to disable the other files, allowing them to write certain hidden settings. This can heavily affect the game as certain rendered elements (like shadows) can be completely disabled.

You can read more about it here: [CryEngine Docs: Using Console and Config Files](https://docs.cryengine.com/display/SDKDOC4/Using+Console+and+Config+Files)

List of all variables: [Console Commands and Variables](https://docs.cryengine.com/plugins/servlet/mobile?contentId=25535264#content/view/9215968)

## How to apply it

If the game does not have a system.cfg file, you'll need to create it and put it in the game's root directory. This should appear instantly when you click "Browse local files" in Steam.

Then you can place the system.cfg file right into the folder. 

[Video PoC](https://youtu.be/nU6kcxZh4eY)
