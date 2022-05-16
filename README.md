# TWRP device tree for Samsung A13 aka a13x

## Kernel source 
Available at https://github.com/corsicanu/android_kernel_samsung_universal850

## How to build
This was tested and it's fully compatible with [minimal manifest twrp](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp).
1. Set up the build environment following instructions from [here](https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp/blob/twrp-11/README.md#getting-started)
2. In the root folder of cloned repo you need to clone the device tree:
```bash
git clone -b android-11.0 https://github.com/TeamWin/android_device_samsung_a13x.git device/samsung/a13x
```
3. To build:
```bash
export ALLOW_MISSING_DEPENDENCIES=true && . build/envsetup.sh && lunch twrp_a13x-eng && mka recoveryimage -j128
```

