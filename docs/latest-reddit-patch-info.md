# About patching Reddit versions 2024.18.0+
---

Starting from Reddit 2024.18.0, [APKTool does not support decoding due to resource obfuscation](https://github.com/ReVanced/revanced-patches/issues/3099).

Currently, the only workaround is to use ARSCLib to skip decoding of obfuscated resources.

There has been a lot of discussion about ARSCLib support, but currently, ARSCLib support is in the development stage.

Fortunately, I had locally saved the code testing the ARSCLib branch last year, and was able to restore it and prepare a patch targeting Reddit 2024.18.0+.

Currently, only the CLI method is available.

Downloading the packages
==

- [ReVanced CLI/ARSCLib](https://github.com/inotia00/revanced-cli-arsclib/releases/latest)
- [ReVanced Patches/ARSCLib](https://github.com/inotia00/revanced-patches-arsclib/releases/latest)
- [ReVanced Integrations](https://github.com/inotia00/revanced-integrations/releases/latest)

(Optional): For simplicity, place the Reddit APK and the packages you downloaded in a single folder.

Using ReVanced CLI (PC)
==

- You can use the option '--rip-lib' to remove unwanted architectures. (e.g. `--rip-lib=x86 --rip-lib=x86_64` ...)
- The option '-l' will show the list of available patches.
- The option '-i' allows you to include patches. (e.g. `-i "Custom branding name for Reddit"` ...)
- The option '-e' allows you to exclude patches. (e.g. `-e "Disable screenshot popup"` ...)

```
java -jar revanced-cli-all.jar \
 -a input.apk \
 -o output \
 -m revanced-integrations.apk \
 --options options.json \
 -b revanced-patches.jar
```

After patching is complete, transfer and install `base.apk` from the ouput directory to your Android device.
