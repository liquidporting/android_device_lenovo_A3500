## TWRP device tree for Lenovo IdeaTab A7-50 (A3500)

Add to `.repo/local_manifests/A3500.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/lenovo/A3500" name="android_device_lenovo_A3500" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_A3500-eng
make -j5 recoveryimage
```
