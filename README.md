# cstrike-modding
This repository contains updated FGDs and fixes to make mapping process easy (at least for me xd) for Counter-Strike: Source.

# Installation
1. If you only need FGDs, go to step 5;
2. If not, then install [Hammer++ for CS:S](https://ficool2.github.io/HammerPlusPlus-Website/download.html) (drop into bin folder, don't launch yet);
3. Download nfn_css_fix.zip and unpack it into Counter-Strike: Source folder with replacing;
4. Create shortcut for Hammer++: add to the object field (first one): `-game "C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Source\cstrike"` (based on where the cstrike folder is located) and launch it;
![screenshot](https://sun1.sibirix.userapi.com/impg/IeKwxjQd8kCls9dACIFrtCvDPRYVR4VRk0znHg/i4LTe1kOjoo.jpg?size=642x828&quality=96&sign=27b5251a9da927f5a4186e90b6b5c909&type=album)
5. Tools -> Options -> Game Configurations -> Game Data files, remove everything and add SECSS.fgd and propper.fgd;

# Usage
- When creating maps, place them into custom folder and create a folder with same name as your .vmf inside it.
- How to embed files:
- 1. Make sure you deleted cubemaps. If you did, then open your map in game and compile them. If not, then the map will have default empty one and there will be no reflections;
- 2. Create a text file called `<your map name>_include.txt` inside `custom/<your map name>` folder;
- 3. Edit it: First line is for relative path, secont for absolute:
```
maps\test_map.txt
C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Source\cstrike\custom\test_map\maps\test_map.txt
materials\test.vmt
C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Source\cstrike\custom\test_map\materials\test.vmt
```
- 4. Save it and try running Embed Files template. Your files should be inside now!

# Credits
- Pinsplash for [updated FGD](https://github.com/Pinsplash/SEFGD);
- Bacardi for [HLMV VPK load fix](https://gamebanana.com/gamefiles/3293);
- ficool2 for [Hammer++](https://ficool2.github.io/HammerPlusPlus-Website/);
- Slartibarty for [Slammin' Source Tools](https://drive.google.com/file/d/1gqmMkHTadUmWBMOqSPSlKRLL1zYvoRsS/view).

**Send a direct message in Discord (notfoundname#3292) or create an issue if you have some problems with it.**