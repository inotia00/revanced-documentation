About Revancify
==

Revancify is a tool for building ReVanced in Termux. It is developed by [@decipher3114](https://github.com/decipher3114). Visit the [Revancify repository](https://github.com/decipher3114/Revancify) for more info.


Installing Revancify for the first time
=

1. Install Termux. [Termux Monet](https://github.com/Termux-Monet/termux-monet/releases) is recommended. Otherwise, use [Termux](https://github.com/termux/termux-app/releases/latest).

2. Open Termux and run this command to install Revancify:

```
curl -sL "https://raw.githubusercontent.com/decipher3114/Revancify/main/install.sh" | bash
```

> [!TIP]
> If the above command doesn't work, use this:
>
> ```
> pkg update -y -o Dpkg::Options::="--force-confnew" && pkg install git -y && git clone --depth=1 https://github.com/decipher3114/Revancify.git && ./Revancify/revancify
> ```


#### Usage
After Revancify is installed, type `revancify` in Termux and press `Enter` to run it.  

> [!TIP]   
> It can also be ran with arguments. See the available arguments with `revancify -h` or `revancify --help`.  

> [!TIP]
> You can also use my shortcut to quickly open Revancify. Find out more [here](https://github.com/inotia00/RevancifyShortcut?tab=readme-ov-file#shortcut-for-revancify).


Patching
==

1. From the Revancify menu, select `Change Source` and select `inotia00`. Then, press `Done`.

> [!NOTE]
> If it is your first time running Revancify, the Change Source menu will open automatically upon installation. So just select `inotia00` and press `Done`.

2. Select `Fetch Tools` to download the latest patch files.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_1.gif" alt="revancify_1"/>


3. Select `Select Patches` to choose patches to include or exclude for the app you want to patch.

- Read [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/information-about-patches.md) for information on patches you may want to include or exclude. Otherwise, just click the `Recommended` button.

> [!IMPORTANT]
> For ROOT YouTube / YT Music installations, the `GmsCore support` patch must be excluded. For non-ROOT installations, the patch must be included.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_2.png" alt="revancify_2" width="400"/>


4. Select `Patch App` and choose the app you want to auto-download and patch.

From the Version Selection Menu, choose the `Auto Select` option or a version labeled `[RECOMMENDED]`.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_3.png" alt="revancify_3" width="400"/>


The version will be downloaded and patching will begin.

> [!NOTE]
> If the download feature doesn't work, follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md). Then, return to Revancify and press `From Storage` to select the APK you downloaded from APKMirror.
>
> <img src="https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_4.png" alt="revancify_4" width="400"/>


5. Install the patched APK when prompted.

> [!TIP]
> For ROOT installations, I recommend also installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/). It prevents automatic updates from the Google Play Store, which prevents crashes from occurring in the ROOT environment.
