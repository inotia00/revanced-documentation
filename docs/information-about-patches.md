# Information about the patches

---

The patch list for each app can be found using these links: 

[**YouTube**](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comgoogleandroidyoutube)

[**YouTube Music**](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comgoogleandroidappsyoutubemusic)

[**Reddit**](https://github.com/inotia00/revanced-patches/tree/revanced-extended?tab=readme-ov-file#-comredditfrontpage)



## Patches that need to be included or excluded depending on the situation:

---

### If you want the ROOT YouTube/YT Music version:

- Exclude the `GmsCore support` patch.

Using CLI: `-e "GmsCore support"`

### If you want a custom app icon:

- Include the `Custom branding icon YouTube` / `Custom branding icon YouTube Music` patch.

Using CLI: `-i "Custom branding icon YouTube"` / `-i "Custom branding icon YouTube Music"`

※ You can choose the custom icon by opening `options.json` in an editor. (Available values: `MMT`, `Revancify Blue`, `Revancify Red`, or you can enter the absolute path where the icon file exists.)

### If you want the official app icon:

- Exclude the `Custom branding icon YouTube` / `Custom branding icon YouTube Music` patch.

Using CLI: `-e "Custom branding icon YouTube"` / `-e "Custom branding icon YouTube Music"`

### If you want a custom app name:

- Include the `Custom branding name YouTube` / `Custom branding name YouTube Music` / `Custom branding name Reddit` patch.

Using CLI: `-i "Custom branding name YouTube"` / `-i "Custom branding name YouTube Music"` / `-i "Custom branding name Reddit"`

※ You can choose the custom app name by opening `options.json` in an editor. (Default: ReVanced Extended)

### If you want the official app name:

- Exclude the `Custom branding name YouTube` / `Custom branding name YouTube Music` / `Custom branding name Reddit` patch.

Using CLI: `-e "Custom branding name YouTube"` / `-e "Custom branding name YouTube Music"` / `-e "Custom branding name Reddit"`

### If you want the standard YouTube theme:

- Exclude the `Theme` and `MaterialYou` patches.

Using CLI: `-e "Theme" -e "MaterialYou"`

### If you want a custom YouTube theme:

(Custom light theme + Custom dark theme)

- Include the `Theme` patch.

- Exclude the `MaterialYou` patch.

Using CLI: `-i "Theme" -e "MaterialYou"`

※ You can choose the custom theme colors by opening `options.json` in an editor and specifying the HEX colors. (Default dark theme: Amoled Black)

### If you want a MaterialYou theme in YouTube (only on Android 12+):

(MaterialYou light theme + MaterialYou dark theme)

- Exclude the `Theme` patch.

- Include the `MaterialYou` patch.

Using CLI: `-e "Theme" -i "MaterialYou"`

### If you want a MaterialYou theme + Custom dark theme in YouTube (only on Android 12+):

(Material light theme + Custom dark theme)

- Include the `Theme` and `MaterialYou` patches.

Using CLI: `-i "Theme" -i "MaterialYou"`

※ You can choose the custom dark theme color by opening `options.json` in an editor and specifying the HEX color. (Default dark theme: Amoled Black)
