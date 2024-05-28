Downloading the packages
==
- [ReVanced CLI](https://github.com/inotia00/revanced-cli/releases/latest)
- [ReVanced Patches](https://github.com/inotia00/revanced-patches/releases/latest)
- [ReVanced Integrations](https://github.com/inotia00/revanced-integrations/releases/latest)

Using ReVanced CLI (PC)
==
1. Make sure your phone is connected

```
adb shell exit
```

2-1. If you plan to use the root variant, check if you have root access
```
adb shell su -c exit
```

2-2. If you plan to use the root variant, copy the ADB device name
```
adb devices
```

2-3. If you plan to use the root variant, please install youtube (or youtube music) on your device first.
```
adb install -r youtube.apk
```
```
adb install -r youtube-music.apk
```

3. Run the CLI
```
# Non-Root
# For YouTube, use the option '--rip-lib' to remove the architecture (e.g. --rip-lib=x86 --rip-lib=x86_64 ...)

java -jar revanced-cli-all.jar patch \
 -c \
 -o revanced.apk \
 -m app-release-unsigned.apk \
 -r revanced-resource-cache \
 --options options.json \
 -b revanced-patches.jar \
 youtube.apk


# Root
# For YouTube, use the option '--rip-lib' to remove the architecture (e.g. --rip-lib=x86 --rip-lib=x86_64 ...)
# In the case of YouTube you want to exclude the patch 'GmsCore support' with the option '-e'.
# The option '-e' allows you to exclude patches (e.g. -e "GmsCore support" -e "Theme" ...).
# The option '-i' allows you to include patches (e.g. -i "MaterialYou" ...)

java -jar revanced-cli-all.jar patch \
 -c \
 -d device-name \
 -o revanced.apk \
 -m app-release-unsigned.apk \
 -r revanced-resource-cache \
 --options options.json \
 -b revanced-patches.jar \
 -e "GmsCore support" \
 --mount \
 youtube.apk
```


If you need the list of patches available, pass in `-l`.