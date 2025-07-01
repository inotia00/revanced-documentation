About Revancify
==

Revancify is a tool for building ReVanced in Termux. It is developed by [@decipher3114](https://github.com/decipher3114). Visit the [Revancify repository](https://github.com/decipher3114/Revancify) for more info.


Installing Revancify for the first time
=

1. Install [Termux](https://github.com/termux/termux-app/releases/latest).

2. Open Termux and run this command to install Revancify:

```
curl -sL https://github.com/decipher3114/Revancify/raw/refs/heads/main/install.sh | bash
```


#### Usage
After Revancify is installed, type `revancify` in Termux and press `Enter` to run it.  

> [!TIP]   
> It can also be ran with arguments. See the available arguments with `revancify -h`.  

> [!TIP]
> You can also use my shortcut to quickly open Revancify. Find out more [here](https://github.com/inotia00/RevancifyShortcut?tab=readme-ov-file#shortcut-for-revancify).


Patching
==

1. From the Revancify menu, select `Change Source` and select `ReVanced-Extended`. Then, press `Done`.

2. Select `Update Assets` to download the latest CLI and patch files.

<img src="/images/revancify_1.gif" width="300"/>


3. Select `Patch App` and choose the app you want to auto-download and patch. From the Version Selection Menu, choose the `Auto Select` option or a version labeled `[RECOMMENDED]`.

<img src="/images/revancify_2.png" width="400"/>

> [!IMPORTANT]
> If there is no `Auto Select` or `[RECOMMENDED]` option, follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md). Then, move the APK you downloaded into `Internal storage/Revancify/Stock`. Then, return to Revancify and press `Import` to import the APK you placed in the `Stock` directory.
>
> <img src="/images/revancify_3.png" width="400"/>

4. Choose patches to include or exclude. If you aren't sure, just press `Recommended`.

- Read [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/information-about-patches.md) for information on patches you may want to include or exclude.

> [!IMPORTANT]
> For ROOT YouTube / YT Music installations, the `GmsCore support` patch must be excluded. For non-ROOT installations, the patch must be included.
>
> <img src="/images/revancify_4.png" width="400"/>

5. After selecting the patches you can configure the patch options (options.json). After they are set to your liking, press `Done` to begin patching.

6. Install the patched APK when prompted. (The patched APK will also be saved in `Internal storage > Revancify > Patched`.)

> [!TIP]
> For ROOT installations, I recommend also installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/). It prevents automatic updates from the Google Play Store, which would cause crashes to occur in the ROOT environment.
