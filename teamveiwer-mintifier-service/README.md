# Teamveiwer Mintifier Service
A service and bash script combination to force the teamveiwer tray icon to use the mint-y theme (teamveiwer will occasionally overwrite icons in the folder the bash script writes to). Designed for linux mint (in about 10 minutes). It's easy, but time consuming, hence the repo. Not affiliated with TeamViewer Germany GmbH.

## Steps

File locations:
Requires Files (nemo) to be run as root. Right click on empty space in a folder, then click "Open as Root".
* tviconreplace.sh goes in `/usr/bin`. Set as executable by going to Properties, Permissions, then check "allow executing file as program."
* tviconreplacer.service goes in `/etc/systemd/system`
* The teamvIntegratedIcons folder goes in `/usr/share/icons`

Commands:
After putting in files in the respective folders, run `systemctl start tviconreplacer.service` then `systemctl enable tviconreplacer.service`. For info on the service (optional), run `systemctl status tviconreplacer.service`. Authenticate as an administrator each time. 
Next:
Reboot you computer if you want, then Profit!

## Troubleshooting 
There are 100% verified no bugs. That said, if one finds its way in, calmly cover said bug with a cup, slip a paper underneath, and release the captured bug outside. 

## Credits
snwh for moka-icon-theme, used by Linux Mint:
https://github.com/snwh/moka-icon-theme
See Licence file for usage rights. 
