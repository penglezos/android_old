## LineageOS 21.0 for K20 Pro/Mi 9T Pro Installation instructions
First time installation:
- Make sure you backup your data
- Install LineageOS recovery via fastboot (or [OrangeFox](https://androidfilehost.com/?fid=4279422670115710816)): `fastboot flash recovery filename.img`
- Now reboot into recovery to verify the installation
- Sideload the latest [Android 11 firmware](https://xiaomifirmwareupdater.com/firmware/raphael/) of your device variant
- Now tap Factory Reset, then Format data / factory reset and continue with the formatting process. This will remove encryption and delete all files stored in the internal storage
- Return to the main menu and reboot into recovery
- Sideload the LineageOS .zip:
On the device, select “Apply Update”, then “Apply from ADB” to begin sideload
On the host machine, sideload the package using: `adb sideload filename.zip` or you can use an USB-OTG device
- Sideload GAPPS (recommended: [MindTheGapps](https://github.com/MindTheGapps/13.0.0-arm64/releases/latest)) (optional step) `adb sideload filename.zip`
- Reboot
- If you face a system bootloop reboot into fastboot mode open terminal and execute `fastboot -w`

Update to newer release:
- Make sure you backup your data
- Boot into recovery 
- Sideload the LineageOS .zip:
On the device, select “Apply Update”, then “Apply from ADB” to begin sideload
On the host machine, sideload the package using: `adb sideload filename.zip` or you can use an USB-OTG device
- Sideload GAPPS (recommended: [MindTheGapps](https://github.com/MindTheGapps/13.0.0-arm64/releases/latest)) (optional step) `adb sideload filename.zip`
- Reboot

Or you can simply download the OTA package update and install it through the updater menu which will promt to LineageOS recovery and flash it for you.

NOTE: Make sure to flash newer recovery with each release to stay updated.
