Information
==
### 1. This document is a guide on how to build ReVanced Extended apps using the RVX Manager.


### 2. To use the RVX Manager, the following conditions must be met:
- Your device must use the arm64-v8a architecture.
- Your device must be running Android 8.0+.



Common
==
### 0. If you are preparing to install in **ROOT environment**, follow the method below
- remove all YouTube / YT Music related modules
- remove directories: `/data/adb/service.d`, `/data/adb/post-fs-data.d`, `/data/adb/revanced`
- reboot device

​
### 1. Check the [README.md](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-json-format) of revanced-patches for supported versions

![support_version_youtube](https://github.com/inotia00/revanced-documentation/blob/main/images/compatible_packages_youtube.png)

→ YouTube

![support_version_music](https://github.com/inotia00/revanced-documentation/blob/main/images/compatible_packages_youtube_music.png)

→ YouTube Music

![support_version_reddit](https://github.com/inotia00/revanced-documentation/blob/main/images/compatible_packages_reddit.png)

→ Reddit

### 2. Download the supported version of YouTube / YouTube Music from APKMirror and **_install it on your device._**

![APKMIRROR](https://github.com/inotia00/revanced-documentation/blob/main/images/apkmirror_youtube.png)

※ You must download the `nodpi` variant, and the architecture must be compatible with the device you plan to install the patched APK on.


### 2-1. When you try to build YouTube/YouTube Music

Install the APK downloaded from APKMirror on your device.

### 2-1. When you try to build Reddit

Do not install APK downloaded from APKMirror on your device.

### 3. Download RVX Manager from GitHub and install it on your device.

[Download RVX Manager](https://github.com/inotia00/revanced-manager/releases/latest)

### 4. Launch RVX Manager, click `Patcher` and then `Select an application`.

![1](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_1.png)


### 4-1. If you want to build YouTube(ROOT) or YouTube Music(ROOT)

![2-1](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_2.png)

If you are building YouTube or YouTube Music in a ROOT environment, click the card for the application you installed.

### 4-2. In other cases

![2-2](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_3.png)

If you want to build Reddit, or YouTube(NON-ROOT) or YouTube Music(NON-ROOT),
Click the 'Storage' button at the bottom right and select the APK downloaded from APKMirror.


### 5. Click `Selected patches` and include or exclude the patches you want

![5](https://github.com/inotia00/revanced-documentation/blob/main/images/rvx_manager_4.png)

- If you don't know what to decide, just click the `Default` button

- When selected, click the `Done` button, and then the `Patch` button


※ Read [this document](https://github.com/inotia00/revanced-documentation/wiki/Options-Information-about-the-patch) for a list of patches you can include or exclude.

※ Read [this document](https://github.com/ReVanced-Extended-Community/Patches-Documentation) to see a screenshot of each patch.


NON-ROOT environment
==
When patching, **include** the following patches:

- **`GmsCore support`**


ROOT environment
==
When patching, **exclude** the following patches:

- **`GmsCore support`**


I recommend installing the [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/) after patching.

※ [Detach Magisk module](https://forum.xda-developers.com/t/module-detach3-detach-market-links.3447494/) prevents automatic updates by Google Playstore. (Prevent crashes from occurring in the ROOT environment)