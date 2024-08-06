Requirements
==

- Your device's architecture must be arm64-v8a, armeabi-v7a, or x86-64.
- Your device must be running Android 8+.


Using RVX Manager
==

1. Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to supply and prepare an APK to patch.


2. Download [RVX Manager](https://github.com/inotia00/revanced-manager/releases/latest) from GitHub and install it on your device.


3. Launch RVX Manager, click `Patcher` and then `Select an application`.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_1.png" alt="rvx_manager_1" width="400"/>


4. (Non-ROOT installations): Click the `Storage` button at the bottom right and select the APK downloaded from APKMirror.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_2.png" alt="rvx_manager_2" width="400"/>


4. (ROOT installations): Click the card for the application you installed.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_3.png" alt="rvx_manager_3" width="400"/>


5. Click `Selected patches` and include or exclude the patches you want.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_4.png" alt="rvx_manager_4" width="400"/>


- Read [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/information-about-patches.md) for information on patches you may want to include or exclude. Otherwise, just click the `Default` button.

> [!IMPORTANT]
> For ROOT YouTube / YouTube Music installations, the `GmsCore support` patch must be excluded. For non-ROOT installations, the patch must be included.

- When satisfied with your patch selection, click the `Done` button, and then the `Patch` button. 


6. Install the patched APK.

> [!TIP]
> For ROOT installations, I recommend also installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/). It prevents automatic updates from the Google Play Store, which prevents crashes from occurring in the ROOT environment.
