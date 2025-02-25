### Pre-installation:

* Required firmware: Android 10  
* Optional gapps (from download page, gapps button)  
* XDA thread [here](https://xdaforums.com/t/unofficial-14-0-crdroid-10-6-for-xperia-xz2-premium-aurora.4685876/)  

### First time installation (clean flash):

* Step 1: Unlock your bootloader at [https://developer.sony.com/open-source/aosp-on-xperia-open-devices/get-started/unlock-bootloader](https://developer.sony.com/open-source/aosp-on-xperia-open-devices/get-started/unlock-bootloader)  
* Step 2: Update to the latest system software if you haven't already; Android 10 or newer is required to install this ROM.  
* Step 3: Download the recovery image and boot into fastboot then run below command to install recovery (replace *boot-xxxxxxxx.img* with the filename for the latest recovery).

```
fastboot flash boot boot-xxxxxxxx.img
```

* Step 4: Now boot to recovery.

```
fastboot reboot recovery
```

**Do not boot into the OS before you flash the ROM! The stock ROM will replace the recovery!!**

* Step 5: Select Apply update from ADB, then use adb sideload to apply the ROM.  
* Step 6: Boot back into recovery if you aren't still in recovery, and select Factory reset.  
* Step 7: Select reboot, and you're done!  

### Manual update installation:

* Step 1: Reboot into recovery - I recommend using the recovery option from Advanced restart menu to do this  
* Step 2: Select "Apply update" and "Apply update from ADB". Plug the device into your computer. If it is not recognized, you can use Google ADB drivers or Sony's ADB drivers. Most will work.  
* Step 3: Download the latest build and use the following command to update, replacing crdroid.zip with the filename of the latest build:

```
adb sideload crdroid.zip
```
