# disable-phantom-procs-killer-miui [NO ROOT] [NO COMPUTER]

**Quick guide to disable phantom process killer on Miui**

## What do you need

[Termux](https://f-droid.org/en/packages/com.termux/) (F-droid)

**Android 12+**

**Stable internet connection**

**A device that is NOT Samsung** 

**16.3 IQ**

yes. thats literally it, no root or no computer required



# Guide

**Enable developer options**

**Enable wireless debugging**

**Go on Termux**
```
pkg install android-tools

```
```

adb pair localhost:[insert your port]
```
```
[ur wifi pairing code]
```
```
adb connect localhost:[your port]
```

if connected, paste these:

```

adb shell "/system/bin/device_config set_sync_disabled_for_tests persistent"
```
```
adb shell "/system/bin/device_config put activity_manager max_phantom_processes 2147483647"
```
```
adb shell settings put global settings_enable_monitor_phantom_procs false
```

**❗dw if the last one gave y a error it will still work.❗**

✅ **you're all done, incase you're wondering, no you don't have to do this everytime you launch a desktop
it's for one tjme**



