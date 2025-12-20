# Recovery Device Tree for Samsung Galaxy S23 Ultra (dm3q)

## To build it: 
```bash
. build/envsetup.sh
lunch twrp_dm3q-eng
mka recoveryimage -j$(nproc --all)
```

## Shared with Samsung SM8550 common device tree: 
https://github.com/samsung-sm8550-cola2261/android_device_samsung_sm8550-common-recovery

## Known Issues
 - Unable to mount, decrypt /data partition
 - Slow charging on recovery
 - No vibration support
 - No ability to flash logical partitions (system, vendor, etc.)

## Special Thanks:
[archer0305](https://github.com/archer0305) for device tree

[Edgars Cīrulis](https://github.com/Edgars-Cirulis) for the prebuilt kernel

[Hunter](https://github.com/devhunter1) for the AVB digest patch
