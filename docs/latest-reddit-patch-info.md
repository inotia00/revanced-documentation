Background
==

Starting from Reddit 2025.40.0, [APKTool does not support decoding due to resource obfuscation](https://github.com/ReVanced/revanced-patches/issues/3099).

Currently, the only workaround is to use ARSCLib to skip decoding of obfuscated resources.

There has been a lot of discussion about ARSCLib support, but currently, ARSCLib support is in the development stage.

Fortunately, I had locally saved the code testing the ARSCLib branch last year, and was able to restore it and prepare a patch targeting Reddit 2025.40.0+.

Currently, only the rvx-builder and CLI support ARSCLib. Below are instructions for both.

Patching Reddit v2025.40.0+
==

## RVX-Builder (PC)

1. Download the [rvx-builder executable](https://github.com/inotia00/rvx-builder/releases/latest) and run it.

2. A GUI will open in your browser. Open the rvx-builder settings and enable the `ARSCLib` toggle. Then, click `Home` and patch a Reddit APK. Refer to this [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/rvx-builder%20(pc).md#using-rvx-builder-windows--macos--linux) for more details.


## RVX-Builder (Android - Termux)

1. Install rvx-builder in Termux and run it as described in [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/rvx-builder%20(android).md#installing-rvx-builder-for-the-first-time).

2. A GUI will open in your browser. Open the rvx-builder settings and enable the `ARSCLib` toggle. Then, press `Home` and patch a Reddit APK. Refer to this [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/rvx-builder%20(android).md#using-rvx-builder-termux) for more details.


## ReVanced CLI (PC)

### Requirements

- x86/x86_64 host architecture
- [Zulu JDK 17](https://www.azul.com/downloads/?version=java-17-lts&package=jdk#zulu) (You can check the installed version by running `java --version` in a terminal)


### Preparing the packages

1. Check the JSON format in the [README.md](https://github.com/inotia00/revanced-patches-arsclib?tab=readme-ov-file#-json-format) of the revanced-patches-arsclib repository to see which app versions are supported.

2. Go to [apkmirror.com](https://www.apkmirror.com/) and download a supported version of Reddit to your PC.

> [!NOTE]
>
> Do not install the APK you downloaded from APKMirror.

3. Download the following packages to your PC:

- [APKEditor](http://github.com/REAndroid/APKEditor/releases/latest) (`.jar` file)
- [ReVanced CLI ARSCLib](https://github.com/inotia00/revanced-cli-arsclib/releases/latest) (`.jar` file)
- [ReVanced Patches ARSCLib](https://github.com/inotia00/revanced-patches-arsclib/releases/latest) (`.jar` file)
- [ReVanced Integrations](https://github.com/inotia00/revanced-integrations/releases/latest) (`.apk` file)

4. (Optional): For simplicity, place the APK and packages you downloaded in a folder named `revanced-extended`.

5. Run the following command to merge the split/bundle Reddit APK into a `.apk`:

```
java -jar APKEditor.jar m -i reddit.apkm
```


### Using ReVanced CLI

- The option '-l' will show the list of available patches.
- The option '-i' allows you to include patches. (e.g. `-i "Custom branding name for Reddit"` ...)
- The option '-e' allows you to exclude patches. (e.g. `-e "Disable screenshot popup"` ...)

```
java -jar revanced-cli-all.jar \
 -a reddit_merged.apk \
 -o output-folder \
 -m revanced-integrations.apk \
 --options options.json \
 -b revanced-patches.jar
```

After patching is complete, install `base.apk` from the `output-folder` folder to your Android device.
