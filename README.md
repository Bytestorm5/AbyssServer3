# AbyssCraft 3 Mod Repo

## Organization

Mods are organized into different branches, effectively working as presets:

`bare-minimum:` The bare minimum mods you need to connect to the server- no client-side optimizations or anything. Don't use this unless you have your own set of cleint-side mods that you want to use.

`performance:` The base pack with optimization mods like Rubidium and Magnesium _(not Optifine bc that breaks things)_.

`pretty:` Includes everything from the performance pack, with extra resourcepacks and mods for aesthetics. **This preset is not done yet.**

## Quick Start

 - [Install Forge](https://files.minecraftforge.net/net/minecraftforge/forge/index_1.18.2.html). You will need version `40.1.79` or higher- you can just pick up the latest version and be fine.

 - Start minecraft on the new Forge installation and make sure it fully loads once with no mods loaded- you technically don't have to do this but its good to make sure its working

 - Select a preset to run from the `branches` menu:

![image](https://user-images.githubusercontent.com/31070777/206109193-2d5e6ea2-2756-481a-bf5a-3ea23068d9cc.png)

Download the branch as a `.zip` file and extract it (windows has this as a base feature):

![image](https://user-images.githubusercontent.com/31070777/206109824-6405eb26-698c-4c8e-8616-ed559645f1a0.png)

 - Move the mods in the `mods` folder into your `.minecraft/mods` folder _(on windows this is located at `%appdata%/.minecraft`- you can copy/paste that into your file explorer path)_
If there are already mods in the mods folder, take them out

 - - If the preset includes a resourcepack, copy the files in the `resourcepacks` folder into your `.minecraft/resourcepacks` folder:

 - For the new forge installation, it's reccomended to set the JVM arguments to the following:

`-XX:+UseG1GC -Xmx6G -Dsun.rmi.dgc.server.gcInterval=2147483646 -XX:+UnlockExperimentalVMOptions -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M`
 
 This will give the game 6GB of RAM and gives it better Garbage Collection parameters than the default. If you understood what that meant do not ask me to explain why because I do not know I copied this from a reddit thread and it works
