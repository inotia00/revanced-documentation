### 1. Check the supported app versions

Check the JSON format in the [README.md](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-json-format) of the revanced-patches repository to see which app versions are supported.

> [!NOTE]
>
> If you want to use ReVanced Patches ARSCLib, check the [README.md](https://github.com/inotia00/revanced-patches-arsclib?tab=readme-ov-file#-json-format) of that repository.


> [!TIP]
> 
> If you are confused by the JSON, here is an explanation:
> - The supported YouTube versions are listed by `com.google.android.youtube`
> - The supported YT Music versions are listed by `com.google.android.apps.youtube.music`
> - The supported Reddit versions are listed by `com.reddit.frontpage`
>
> If there are no listed supported versions for one of the apps it means that the patches are not constrained to specific versions, and that a wide range of versions are expected to work.


### 2. Download a supported version of YouTube / YT Music / Reddit

Go to [apkmirror.com](https://www.apkmirror.com/) and download a supported version of the app you want to patch.

<img src="/images/apkmirror_youtube.png" width="700"/>

The architecture of the APK must be compatible with the device you plan to install the patched APK on.

> [!NOTE]
> ### If you are patching Reddit:
>
> Do not install the APK you downloaded from APKMirror. (Reddit should not be mounted.)


> [!NOTE]
> ### If you are patching Reddit with the RVX Manager:
> 
> If you want to patch a Reddit version newer than 2024.29.0 with the RVX Manager, you will need to convert the split/bundle APK (`.apkm`, `.apks`, `.xapk`, etc.) into a `.apk` using an anti-splitting tool, such as [AntiSplit M](https://github.com/AbdurazaaqMohammed/AntiSplit-M). Note that Reddit versions 2025.40.0 and newer can only be patched using [ARSCLib](https://github.com/inotia00/revanced-documentation/blob/main/docs/latest-reddit-patch-info.md).


> [!NOTE]
> ### If you are preparing to install in a ROOT environment:
>
> 1. Remove all YouTube related modules.
> 2. Remove the following directories: `/data/adb/service.d`, `/data/adb/post-fs-data.d`, `/data/adb/revanced`
> 3. Reboot device. 
> 4. Install the YouTube / YT Music APK you downloaded from APKMirror. 
