Requirements
==

- An Android 8+ device (to install the patched APK on)

> [!NOTE]
> ### If you are preparing to install in a ROOT environment:
>
> Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to prepare the device for a mount installation. Note that the APK from APKMirror that you install must be the same version as the APK you will patch.
>
> You will also need your Android device connected to your PC via ADB.


Using RVX Builder (Windows / MacOS / Linux)
==

1. Download the [rvx-builder executable](https://github.com/inotia00/rvx-builder/releases/latest) and run it.

> [!TIP]
>
> If you encounter an error, please refer to [this issue](https://github.com/inotia00/rvx-builder/issues/7). If your issue is not dicussed there, please report it on the [GitHub issues page](https://github.com/inotia00/rvx-builder/issues).

2. A GUI will open in your browser. Click `Start patching`. After the dependencies are downloaded, click `Continue`.

3. Select the app you want to patch, or upload the APK.

4. Select the patches you want to include.

- Read [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/information-about-patches.md) for information on patches you may want to include or exclude. Otherwise, just click the `Select All` button to select all Default patches.

> [!IMPORTANT]
>
> For ROOT YouTube / YT Music installations, the `GmsCore support` patch must be excluded. For non-ROOT installations, the patch must be included.

5. If you did not upload an APK in step 3, a menu will appear where you can choose the version of the app to patch. Select the first option, marked `(AUTO SELECTION)`, or select a version marked as `(suggested)`. After the APK is downloaded, click `Continue` and wait for patching to complete.

6. For non-ROOT installations, install the patched APK from the `revanced` folder to your Android device. The `revanced` folder will be in the same directory as the rvx-builder executable. For ROOT installations, the app will be mounted automatically.

> [!TIP]
> For ROOT installations, I recommend also installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/). It prevents automatic updates from the Google Play Store, which prevents crashes from occurring in the ROOT environment.


___
- [How to use rvx-builder on Android](https://github.com/inotia00/revanced-documentation/blob/main/docs/rvx-builder%20(android).md)