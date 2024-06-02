Requirements
==

- Your device must use the arm64-v8a architecture.
- Your device must be running Android 8+.


Using RVX Manager
==

1. Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to supply and prepare an APK to patch.


2. Download [RVX Manager](https://github.com/inotia00/revanced-manager/releases/latest) from GitHub and install it on your device.


3. Launch RVX Manager, click `Patcher` and then `Select an application`.

![1](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_1.png)


4. (Non-ROOT installations): Click the `Storage` button at the bottom right and select the APK downloaded from APKMirror.

![2](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_2.png)

4. (ROOT installations): Click the card for the application you installed.

![3](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_3.png)


5. Click `Selected patches` and include or exclude the patches you want.

![4](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_4.png)

- Read [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/information-about-patches.md) for information on patches you may want to include or exclude. Otherwise, just click the `Default` button.

> For ROOT YouTube / YouTube Music installations, the `GmsCore support` patch must be excluded. For non-ROOT installation, the patch must be included.

- When satisfied with your patch selection, click the `Done` button, and then the `Patch` button. 


6. Install the patched APK.

> For ROOT installations, I recommend also installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/). It prevents automatic updates from Google Playstore, which prevents crashes from occurring in the ROOT environment.