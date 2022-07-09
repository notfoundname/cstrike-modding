# cstrike-modding
This repository contains files and information for easier and less painful modding and mapping of Counter-Strike: Source (probably it can apply to other Source-sdk-MP2013 based games).

# Installation
1. Drag & Drop everything into Counter-Strike: Source folder (where cstrike, hl2, bin, platform and hl2.exe are located);
2. Install [Hammer++ for CS:S](https://ficool2.github.io/HammerPlusPlus-Website/download.html) (drop into bin folder, don't launch yet);
3. Install [Slammin' Source Tools](https://drive.google.com/file/d/1gqmMkHTadUmWBMOqSPSlKRLL1zYvoRsS/view) (drop into bin folder with file replacing);
4. Create shortcut for Hammer++: add to the object field (first one): `-game "C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Source\cstrike"` (based on where the cstrike folder is located);
[screenshot](https://sun1.sibirix.userapi.com/impg/IeKwxjQd8kCls9dACIFrtCvDPRYVR4VRk0znHg/i4LTe1kOjoo.jpg?size=642x828&quality=96&sign=27b5251a9da927f5a4186e90b6b5c909&type=album)
5. Launch Hammer++, Tools -> Options -> Game Configurations -> Game Data files, remove everything and add SECSS.fgd and propper.fgd;
6. For better lightning, add `-ambientocclusion -worldtextureshadows -translucentshadows` to parameters of VVIS;
7. Add to compilation AFTER BSP copying and create (mapname).txt inside maps folder and fill it with file paths you need to embed. Every first line goes for what path will a file have inside a BSP and every second goes for absolute path to file (do not paste quotes):
```
C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Source\bin\bspzip.exe
-addlist $bspdir\$file $bspdir\$file.txt $bspdir\$file
```
And for just to be sure about contents:
```
C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Source\bin\bspzip.exe
-dir $bspdir\$file
```
8. Have fun, maybe.

# Credits
- Pinsplash for updated FGD;
- Bacardi for HLMV VPK load fix;
- ficool2 for Hammer++;
- Slartibarty for Slammin' Source Map Tools.

**Send a direct message in Discord (notfoundname#3292) or create an issue if you have some problems with it.**