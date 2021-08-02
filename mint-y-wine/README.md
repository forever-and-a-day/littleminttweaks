# Mint-Y Wine Theming 

A modification to the Wine registry to make wine applications use a non-ugly Mint-Y esque color palette. Credit to Minio on the [Ubuntu forums](https://ubuntuforums.org/showthread.php?t=55286) for the info!

![mint-y-winetheme](https://user-images.githubusercontent.com/10383240/127800587-01444b11-5488-4992-ba17-930886937fad.png)

### Usage:
1. Copy the contents of user.reg.txt to your clipboard. 
2. Open `~/.wine/user.reg` in Text Editor (xed).
3. Replace all the text from the line starting with `[Control Panel\\Colors]` to the line starting with `"WindowText"=` with the contents of your clipboard
4. Remove any extra lines if preferred. 
5. Restart all Wine applications using this version of Wine. 

### Notes:
The Proton (valve Wine fork for games) registry may be more difficult to find. You may want to try using `grep -r "WINE REGISTRY"` in your steam installation directory or external library folder. Each game/app's file must be updated. Other tools like playonlinux that use a copy of Wine for every sandboxed app will usually require similar steps. 
