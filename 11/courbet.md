### Pre-installation:

* Make sure you have latest firmware available [here](https://xmfirmwareupdater.com/firmware/courbet/) for your country.
* Gapps package (optional) [here](https://sourceforge.net/projects/crdroid/files/gapps)
* Orangefox recovery zip [here](https://t.me/melo159roms/177)
* A pc with platform-tools working (adb/fastboot)

### First time installation (clean flash):

* Flash Orangefox recovery with the custom recovery you already have and reboot to it
* Format data (typing "yes" to remove everything included encryption)
* Enable sideloading in recovery settings
* Sideload crdroid.zip

```
adb sideload path/to/crdroid.zip
```
* Optionally sideload gapps.zip

```
adb sideload path/to/gapps.zip
```
* Reboot system and enjoy crDroid!!

### Update installation (by device itself):

* Download updated crDroid package
* Download updated gapps package if you had them
* Reboot recovery
* Flash crdroid.zip
* Flash gapps.zip if you had them
* Wipe Dalvik/art cache and /cache
* Reboot system

### Update installation (by pc)

* Download updated crDroid package
* Download updated gapps package if you had them
* Reboot recovery
* Activate sideload
* Sideload crdroid.zip

```
adb sideload path/to/crdroid.zip
```
* if you had gapps, re-enable sideload and sideload gapps.zip

```
adb sideload path/to/gapps.zip
```
* Wipe Dalvik/art cache and /cache
* Reboot system and enjoy your updated crDroid!!
