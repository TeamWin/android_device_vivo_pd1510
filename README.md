## TWRP device tree for Vivo Y51L (pd1510)

## Link to the kernel source :-
```xml
https://github.com/sheikhshahnawaz41299/android_kernel_vivo_msm8916.git



```

Add to `.repo/local_manifests/pd1510.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project name="sheikhshahnawaz41299/android_device_vivo_pd1510-twrp" path="device/vivo/pd1510"  remote="github" revision="twrp_8.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```
 source build/envsetup.sh
export ALLOW_MISSING_DEPENDENCIES=true
export LC_ALL="C"
lunch omni_pd1510-eng && mka recoveryimage
```

