### 1. Check the supported app versions

Check the JSON format in the [README.md](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-json-format) of the revanced-patches repository to see which app versions are supported.

> [!TIP]
> 
> If you are confused by the JSON, here is an explanation:
> - The supported YouTube versions are listed by `com.google.android.youtube`.
> - The supported YT Music versions are listed by `com.google.android.apps.youtube.music`.
> - The supported Reddit versions are listed by `com.reddit.frontpage`.
>
> If there are no listed supported versions for one of the apps it means that the patches are not constrained to specific versions, and that a wide range of versions are expected to work.


### 2. Download a supported version of YouTube / YT Music / Reddit

Go to [apkmirror.com](https://www.apkmirror.com/) and download a supported version of the app you want to patch.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/apkmirror_youtube.png" alt="apkmirror_youtube" width="700"/>


You must download the `nodpi` variant, and the architecture must be compatible with the device you plan to install the patched APK on.

> [!NOTE]
> ### If you are patching Reddit:
>
> Do not install the Reddit APK you downloaded from APKMirror (even if installing in a ROOT environment).

> [!NOTE]
> ### If you are preparing to install in a ROOT environment:
>
> 1. Remove all YouTube related modules.
> 2. Remove the following directories: `/data/adb/service.d`, `/data/adb/post-fs-data.d`, `/data/adb/revanced`
> 3. Reboot device. 
> 4. Install the YouTube / YT Music APK you downloaded from APKMirror. 
