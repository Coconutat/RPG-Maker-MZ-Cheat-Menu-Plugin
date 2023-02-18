RPG Maker MZ Cheat Menu Plugin
==============================
So, what is the difference between this fork version and the (original version)[https://github.com/emerladCoder/RPG-Maker-MV-Cheat-Menu-Plugin]?  
In fact, there is no difference.    
The original version is work fine.But RPG Maker MZ Game change js path.So I need to fix the Patcher Program and script path.  
**Thank the original author [emerladCoder](https://github.com/emerladCoder) very much**.Without this author, I can't easily adapt just by modifying a few lines of characters. **Thanks again**.  

Tested game:(Need Know What Know)[https://steamdb.info/app/2150870/]

***  
**Install**  
Type 1 : Pure manual operation  
1. Find the folder named js in GameFolder. 
2. Copy the js folder under folder Cheat_Menu to your game directory.
3. Use Notepad/ [Notepad2](https://github.com/zufuliu/notepad2) / [Noetpad3](https://github.com/rizonesoft/Notepad3) / [Notepad--](https://github.com/cxasm/notepad--) to open main.js.
4. Find `const scriptUrls =` field.  
For example:  
````
const scriptUrls = [
    "js/libs/pixi.js",
    "js/libs/pako.min.js",
    "js/libs/localforage.min.js",
    "js/libs/effekseer.min.js",
    "js/libs/vorbisdecoder.js",
    "js/rmmz_core.js",
    "js/rmmz_managers.js",
    "js/rmmz_objects.js",
    "js/rmmz_scenes.js",
    "js/rmmz_sprites.js",
    "js/rmmz_windows.js",
    "js/plugins.js"
    ];
````  
5. Add the Cheat Menu path in `const scriptUrls =` area.
For example:  
````
const scriptUrls = [
    "js/libs/pixi.js",
    "js/libs/pako.min.js",
    "js/libs/localforage.min.js",
    "js/libs/effekseer.min.js",
    "js/libs/vorbisdecoder.js",
    "js/rmmz_core.js",
    "js/rmmz_managers.js",
    "js/rmmz_objects.js",
    "js/rmmz_scenes.js",
    "js/rmmz_sprites.js",
    "js/rmmz_windows.js",
    "js/plugins.js",
	"js/plugins/Cheat_Menu.js"
];
````  
You can notice an extra line.  
***
Type 2 : There is nothing for the time being.
***

Any other information same as [original version](https://github.com/emerladCoder/RPG-Maker-MV-Cheat-Menu-Plugin).