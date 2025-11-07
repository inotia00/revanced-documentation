Requirements
==

- x86/x86_64 host architecture
- [Zulu JDK 17](https://www.azul.com/downloads/?version=java-17-lts&package=jdk#zulu) (You can check the installed version by running `java --version` in a terminal)
- ADB (only required for ROOT installations)


Preparing the packages
==

1. Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to supply and prepare an APK to patch. You can supply a full APK (`.apk`) or a split/bundle APK (`.apkm`, `.apks`, `.xapk`, etc.).

2. Download the following packages to your PC:

- [ReVanced CLI](https://github.com/inotia00/revanced-cli/releases/latest) (`.jar` file)
- [ReVanced Patches](https://github.com/inotia00/revanced-patches/releases/latest) (`.rvp` file)

3. (Optional): For simplicity, place the APK and packages you downloaded in a folder named `revanced-extended`.

Using ReVanced CLI (PC)
==

## Non-ROOT installations

**Running the CLI:**

- For YouTube (and Reddit), use the option '--rip-lib' to remove unwanted architectures. (e.g. `--rip-lib=x86 --rip-lib=x86_64` ...)
- The option '-d' allows you to disable patches. (e.g. `-d "Theme"` ...)
- The option '-e' allows you to enable patches. (e.g. `-e "MaterialYou"` `-e "GmsCore support"` ...)
- The option 'list-patches' will show the list of available patches. (e.g. `java -jar revanced-cli.jar list-patches patches.rvp` ...)
- The option 'options' allows you to generate options file. (e.g. `java -jar revanced-cli.jar options patches.rvp` ...)
- The option 'patches' allows you to generate patches file. (e.g. `java -jar revanced-cli.jar patches patches.rvp` ...)

```
# Change filenames as needed

java -jar revanced-cli-all.jar patch \
 -p patches.rvp \
 --legacy-options=options.json \
 --purge \
 -o revanced-extended.apk \
 input.apk
```

> [!NOTE]
> 
> If using a split/bundle APK, be sure to specify the file extension for the input APK (e.g. `input.apkm`, `input.apks`, `input.xapk`, etc.). 

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

> **If you haven't done so already, install YouTube / YT Music on your device:**
> ```
> # Change filenames as needed
> 
> adb install -r input.apk
> ```

**4. Running the CLI:**

- For YouTube, use the option '--rip-lib' to remove unwanted architectures. (e.g. `--rip-lib=x86 --rip-lib=x86_64` ...)
- For ROOT installs, you must disable the 'GmsCore support' patch using the option '-d'.
- The option '-d' allows you to disable patches. (e.g. `-d "GmsCore support"` `-d "Theme"` ...)
- The option '-e' allows you to enable patches. (e.g. `-e "MaterialYou"` ...)
- The option 'list-patches' will show the list of available patches. (e.g. `java -jar revanced-cli.jar list-patches patches.rvp` ...)
- The option 'options' allows you to generate options file. (e.g. `java -jar revanced-cli.jar options patches.rvp` ...)
- The option 'patches' allows you to generate patches file. (e.g. `java -jar revanced-cli.jar patches patches.rvp` ...)

```
# Change filenames as needed

java -jar revanced-cli-all.jar patch \
 -d device-name \
 -p patches.rvp \
 --legacy-options=options.json \
 --purge \
 -d "GmsCore support" \
 --mount \
 -o revanced-extended.apk \
 input.apk
```

> [!NOTE]
> 
> If using a split/bundle APK, be sure to specify the file extension for the input APK (e.g. `input.apkm`, `input.apks`, `input.xapk`, etc.).

> [!TIP]
> I recommend also installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/). It prevents automatic updates from the Google Play Store, which would cause crashes to occur in the ROOT environment.
