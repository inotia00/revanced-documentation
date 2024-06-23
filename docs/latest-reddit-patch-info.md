# About patching Reddit versions 2024.18.0+
---

Starting from Reddit 2024.18.0, [APKTool does not support decoding due to resource obfuscation.](https://github.com/ReVanced/revanced-patches/issues/3099)

Currently, the only workaround is to use ARSCLib to skip decoding of obfuscated resources.

There has been a lot of discussion about ARSCLib support, but currently, ARSCLib support is in the development stage.

Fortunately, I had locally saved the code testing the ARSCLib branch last year, and was able to restore it and prepare a patch targeting Reddit 2024.18.0+.

Currently, only the CLI method is available.

Downloading the packages
==
- [ReVanced CLI/ARSCLib](https://github.com/inotia00/revanced-cli/releases/tag/v2.21.2-arsclib)
- [ReVanced Patches/ARSCLib](https://github.com/inotia00/revanced-patches/releases/tag/v2.175.0-arsclib)
- [ReVanced Integrations](https://github.com/inotia00/revanced-integrations/releases/latest)

Using ReVanced CLI (PC)
==
1. Make sure your phone is connected

```
adb shell exit
```

2. Run the CLI
```
java -jar revanced-cli-all.jar \
 -a reddit.apk \
 -o revanced \
 -m app-release-unsigned.apk \
 --options options.json \
 -b revanced-patches.jar
```

3. Move to the `revanced` directory and install `base.apk`
