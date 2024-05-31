Requirements
==

- An Android 8+ device (to install the patched APK on)

**PC:**
- x86/x86_64 host architecture
- Zulu JDK 17
- ADB (only required for ROOT installations)


Downloading the packages
==

1. Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to supply an APK to patch.

2. Download the following packages to your PC:
- [ReVanced CLI](https://github.com/inotia00/revanced-cli/releases/latest)
- [ReVanced Patches](https://github.com/inotia00/revanced-patches/releases/latest)
- [ReVanced Integrations](https://github.com/inotia00/revanced-integrations/releases/latest)


Using ReVanced CLI (PC)
==

## Non-ROOT installations

**Running the CLI:**

- For YouTube and Reddit, use the option '--rip-lib' to remove unwanted architectures. (e.g. `--rip-lib=x86 --rip-lib=x86_64` ...)
- The option '-l' will show the list of available patches.
- The option '-e' allows you to exclude patches. (e.g. `-e "Theme"` ...)
- The option '-i' allows you to include patches. (e.g. `-i "MaterialYou"` `-i "GmsCore support"` ...)


```
java -jar revanced-cli-all.jar patch \
 -c \
 -o revanced.apk \
 -m app-release-unsigned.apk \
 -r revanced-resource-cache \
 --options options.json \
 -b revanced-patches.jar \
 youtube.apk

```

## ROOT installations

**1. Make sure your phone is connected to ADB:**
```
adb shell exit
```

**2. Check if you have root access:**
```
adb shell su -c exit
```

**3. Copy the ADB device name:**
```
adb devices
```

> **If you haven't done so already, install YouTube / YouTube Music on your device:**
> ```
> adb install -r youtube.apk
> ```
> ```
> adb install -r youtube-music.apk
> ```

**4. Running the CLI:**

- For YouTube, use the option '--rip-lib' to remove unwanted architectures. (e.g. `--rip-lib=x86 --rip-lib=x86_64` ...)
- For ROOT installs, you must exclude the 'GmsCore support' patch using the option '-e'.
- The option '-e' allows you to exclude patches. (e.g. `-e "GmsCore support"` `-e "Theme"` ...)
- The option '-i' allows you to include patches. (e.g. `-i "MaterialYou"` ...)
- The option '-l' will show the list of available patches.


```
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
