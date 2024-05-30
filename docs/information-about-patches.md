Options: Information about the patch

==

### [YouTube](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comgoogleandroidyoutube)

### [YouTube Music](https://github.com/inotia00/revanced-patches/tree/revanced-extended#-comgoogleandroidappsyoutubemusic)

Patches that need to be included or excluded depending on the situation

==

### If you want the ROOT version:

- Don't Select GmsCore support

Using CLI: `-e "GmsCore support"`

### If you want Custom App Icon:

- Select Custom Branding Icon YouTube / Custom Branding Icon YouTube Music

Using CLI: `-i "Custom branding icon YouTube"` `-i "Custom branding icon YouTube Music"`

※ You can change the app icon directly by opening `options.json` in an editor. (Available values: `MMT`, `Revancify Blue`, `Revancify Red`, and you can also enter the absolute path where the icon file exists.)

### If you want Original App Icon:

- Don't Select Custom Branding Icon YouTube / Custom Branding Icon YouTube Music

Using CLI: `-e "Custom branding icon YouTube"` `-e "Custom branding icon YouTube Music"`

### If you want Custom App Name:

- Select Custom Branding Name YouTube / Custom Branding Name YouTube Music

Using CLI: `-i "Custom branding name YouTube"` `-i "Custom branding name YouTube Music"`

※ You can change the app name directly by opening `options.json` in an editor. (Default: ReVanced Extended)

### If you want Original App Name:

- Don't Select Custom Branding Name YouTube / Custom Branding Name YouTube Music

Using CLI: `-e "Custom branding name YouTube"` `-e "Custom branding name YouTube Music"`

### If you want Stock YouTube Theme:

- Don't Select Theme

- Don't Select MaterialYou

Using CLI: `-e "Theme" -e "MaterialYou"`

### If you want Custom Themes:

(Custom Light Theme + Custom Dark theme)

- Select Theme

- Don't Select MaterialYou

※ You can change the theme colors directly by opening `options.json` in an editor and specifying a HEX color. (Default dark theme: Amoled Black)

Using CLI: `-i "Theme" -e "MaterialYou"`

### If you want MaterialYou Theme (Only for Android 12+):

(Material Light Theme + Material Dark Theme)

- Don't Select Theme

- Select MaterialYou

Using CLI: `-e "Theme" -i "MaterialYou"`

### If you want MaterialYou Theme (Only for Android 12+) + Custom Dark Theme:

(Material Light Theme + Custom Dark Theme)

- Select Theme

- Select MaterialYou

※ You can change the dark theme color directly by opening `options.json` in an editor and specifying a HEX color. (Default: Amoled Black)

Using CLI: `-i "Theme" -i "MaterialYou"`
