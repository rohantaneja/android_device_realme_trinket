TWRP Device configuration for _trinket_
==============
realme 5 series (codenamed _"trinket"_) is mid-range budget smartphone from OPPO.
realme 5 was announced and released in August 2019.

### TO-DO
```
* init_trinket - unified for RMX1911, RMX1927, RMX2030
* TW_SKIP_COMPATIBILITY_CHECK - skip compatiblity.zip check for OTAs - unofficial for now
```
### Build Instructions
Add project path to .repo/manifest.xml:
```xml
<project path="device/realme/trinket" name="rohantaneja/android_device_realme_trinket" remote="github" revision="twrp-9.0" />
```

To build execute following instructions:
```
. build/envsetup.sh
lunch omni_trinket-eng
mka recoveryimage ALLOW_MISSING_DEPENDENCIES=true

# To flash and test the build
fastboot boot out/target/product/trinket/recovery.img
```

### Credits
```
- mauronofrio (ginkgo - twrp bringup)
- ganeshi4u (RMX1911 bringup)
```
