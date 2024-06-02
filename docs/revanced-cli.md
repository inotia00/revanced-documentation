Requirements
==

- An Android 8+ device (to install the patched APK on)

**PC:**
- x86/x86_64 host architecture
- [Zulu JDK 17](https://www.azul.com/downloads/?version=java-17-lts&package=jdk#zulu)
- ADB (only required for ROOT installations)


Preparing the packages
==

1. Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to supply an APK to patch.

2. Download the following packages to your PC:
- [ReVanced CLI](https://github.com/inotia00/revanced-cli/releases/latest)
- [ReVanced Patches](https://github.com/inotia00/revanced-patches/releases/latest) (`.jar`file)
- [ReVanced Integrations](https://github.com/inotia00/revanced-integrations/releases/latest)

3. (Optional): For simplicity, place the APK you downloaded from APKMirror and the packages you downloaded in a folder named `revanced-extended`.


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
 -b revanced-patches.jar \
 -m revanced-integrations.apk \
 --options options.json \
 -p \
 -o revanced-extended.apk \
 input.apk
```

After patching is complete, install `revanced-extended.apk` from the `revanced-extended` folder to your Android device.

## ROOT installations

**1. Make sure your phone is connected to ADB**

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
> adb install -r input.apk
> ```

**4. Running the CLI:**

- For YouTube (and Reddit), use the option '--rip-lib' to remove unwanted architectures. (e.g. `--rip-lib=x86 --rip-lib=x86_64` ...)
- For ROOT installs, you must exclude the 'GmsCore support' patch using the option '-e'.
- The option '-e' allows you to exclude patches. (e.g. `-e "GmsCore support"` `-e "Theme"` ...)
- The option '-i' allows you to include patches. (e.g. `-i "MaterialYou"` ...)
- The option '-l' will show the list of available patches.


```
java -jar revanced-cli-all.jar patch \
 -d device-name \
 -b revanced-patches.jar \
 -m revanced-integrations.apk \
 --options options.json \
 -p \
 -e "GmsCore support" \
 --mount \
 -o revanced-extended.apk \
 input.apk

```
