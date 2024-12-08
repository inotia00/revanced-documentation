Information about the patches
==

The patch list for each app can be found using these links: 

[**YouTube**](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comgoogleandroidyoutube)

[**YouTube Music**](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comgoogleandroidappsyoutubemusic)

[**Reddit**](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comredditfrontpage)



Patches that need to be enabled or disabled depending on the situation:
==

### If you want the ROOT YouTube/YT Music version:

- Disable the `GmsCore support` patch.

Using CLI: `-d "GmsCore support"`

### If you want a custom app icon:

- Enable the `Custom branding icon YouTube` / `Custom branding icon YouTube Music` patch.

Using CLI: `-e "Custom branding icon YouTube"` / `-e "Custom branding icon YouTube Music"`

※ You can choose the custom icon by opening `options.json` in an editor. (Available values: `MMT`, `Revancify Blue`, `Revancify Red`, or you can enter the absolute path where the icon file exists.)

### If you want the official app icon:

- Disable the `Custom branding icon YouTube` / `Custom branding icon YouTube Music` patch.

Using CLI: `-d "Custom branding icon YouTube"` / `-d "Custom branding icon YouTube Music"`

### If you want a custom app name:

- Enable the `Custom branding name YouTube` / `Custom branding name YouTube Music` / `Custom branding name Reddit` patch.

Using CLI: `-e "Custom branding name YouTube"` / `-e "Custom branding name YouTube Music"` / `-e "Custom branding name Reddit"`

※ You can choose the custom app name by opening `options.json` in an editor. (Default: ReVanced Extended)

### If you want the official app name:

- Disable the `Custom branding name YouTube` / `Custom branding name YouTube Music` / `Custom branding name Reddit` patch.

Using CLI: `-d "Custom branding name YouTube"` / `-d "Custom branding name YouTube Music"` / `-d "Custom branding name Reddit"`

### If you want the standard YouTube theme:

- Disable the `Theme` and `MaterialYou` patches.

Using CLI: `-d "Theme" -d "MaterialYou"`

### If you want a custom YouTube theme:

(Custom light theme + Custom dark theme)

- Enable the `Theme` patch.

- Disable the `MaterialYou` patch.

Using CLI: `-e "Theme" -d "MaterialYou"`

※ You can choose the custom theme colors by opening `options.json` in an editor and specifying the HEX colors. (Default dark theme: Amoled Black)

### If you want a MaterialYou theme in YouTube (only on Android 12+):

(MaterialYou light theme + MaterialYou dark theme)

- Disable the `Theme` patch.

- Enable the `MaterialYou` patch.

Using CLI: `-d "Theme" -e "MaterialYou"`

### If you want a MaterialYou theme + Custom dark theme in YouTube (only on Android 12+):

(Material light theme + Custom dark theme)

- Enable the `Theme` and `MaterialYou` patches.

Using CLI: `-e "Theme" -e "MaterialYou"`

※ You can choose the custom dark theme color by opening `options.json` in an editor and specifying the HEX color. (Default dark theme: Amoled Black)
