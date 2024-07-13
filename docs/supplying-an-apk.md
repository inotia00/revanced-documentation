### 1. Check the supported app versions

Check the JSON format in the [README.md](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-json-format) of the revanced-patches repository to see which app versions are supported.

> [!NOTE]
> The screenshots below usually do **not** show the currently supported versions. They only demonstrate which sections of the JSON shows the supported versions for each app. Check the [README.md](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-json-format) to see the currently supported versions.

YouTube:

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/compatible_packages_youtube.png" alt="compatible_packages_youtube" width="400"/>


YouTube Music:

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/compatible_packages_youtube_music.png" alt="compatible_packages_youtube_music" width="400"/>


Reddit:

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/compatible_packages_reddit.png" alt="compatible_packages_reddit" width="400"/>


### 2. Download a supported version of YouTube / YouTube Music / Reddit

Go to [apkmirror.com](https://www.apkmirror.com/) and download a supported version of the app you want to patch.

<img src="https://github.com/inotia00/revanced-documentation/blob/main/images/apkmirror_youtube.png" alt="apkmirror_youtube" width="700"/>


You must download the `nodpi` variant, and the architecture must be compatible with the device you plan to install the patched APK on.

> [!NOTE]
> ### If you are patching Reddit:
>
> Do not install the Reddit APK you downloaded from APKMirror (even if installing in a ROOT environment).

> [!NOTE]
> ### If you are preparing to install in a **ROOT environment**:
>
> 1. Remove all YouTube related modules.
> 2. Remove the following directories: `/data/adb/service.d`, `/data/adb/post-fs-data.d`, `/data/adb/revanced`
> 3. Reboot device. 
> 4. Install the YouTube / YouTube Music APK you downloaded from APKMirror. 
