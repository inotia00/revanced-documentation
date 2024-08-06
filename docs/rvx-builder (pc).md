Requirements
==

- An Android 8+ device (to install the patched APK on)


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
> For ROOT YouTube / YT Music installations, the `GmsCore support` patch must be excluded. For non-ROOT installations, the patch must be included.

5. If you did not upload an APK in step 3, a menu will appear where you can choose the version of the app to patch. Select the first option, marked `(AUTO SELECTION)`, or select a version marked as `(suggested)`. After the APK is downloaded, click `Continue`.

6. After patching is complete, install the patched APK from the `revanced` folder to your Android device. The `revanced` folder will be in the same directory as the rvx-builder executable.

> [!NOTE]
> ### If you are preparing to install in a ROOT environment:
>
> 1. Remove all YouTube related modules.
> 2. Remove the following directories: `/data/adb/service.d`, `/data/adb/post-fs-data.d`, `/data/adb/revanced`
> 3. Reboot device. 
> 4. Install the unpatched YouTube / YT Music APK that is in the `revanced` folder before installing the patched APK.



Using RVX Builder (Android - termux)
==
- [How to use rvx builder on Android](https://github.com/inotia00/revanced-documentation/blob/main/docs/rvx-builder.md)