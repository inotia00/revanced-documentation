Installing RVX Builder for the first time
==

1. Install [Termux Monet](https://github.com/HardcodedCat/termux-monet/releases/latest) or [Termux](https://github.com/termux/termux-app/releases/latest).

2. Open Termux and run these commands:

```
curl -sLo rvx-builder.sh https://raw.githubusercontent.com/inotia00/rvx-builder/revanced-extended/android-interface.sh && chmod +x rvx-builder.sh && ./rvx-builder.sh
```

> [!TIP]
>
> If an error occurs, enter it line by line: 
>
> ```
> curl -sLo rvx-builder.sh https://raw.githubusercontent.com/inotia00/rvx-builder/revanced-extended/android-interface.sh
> ```
> ```
> chmod +x rvx-builder.sh
> ```
> ```
> ./rvx-builder.sh
> ```

> [!NOTE]
>
> During initial installation, Termux may ask if you want to update additional packages. (Enter `Y` or `N`.)

After installing, rvx-builder will run automatically.


Using RVX Builder (Termux)
==

> [!NOTE]
> ### If you are preparing to install in a ROOT environment:
>
> Follow the steps on [this page](https://github.com/inotia00/revanced-documentation/blob/main/docs/supplying-an-apk.md) to prepare the device for a mount installation. Note that the APK from APKMirror that you install must be the same version as the APK you will patch.
>
> Also, Termux must have superuser permissions granted.


1. Run rvx-builder with either of these commands in Termux:

```
rvx
```
or
```
./rvx-builder.sh run
```

2. A GUI will open in your browser. Click `Start patching`. After the dependencies are downloaded, click `Continue`.

3. Select the app you want to patch, or upload the APK.

4. Select the patches you want to include.

- Read [this document](https://github.com/inotia00/revanced-documentation/blob/main/docs/information-about-patches.md) for information on patches you may want to include or exclude. Otherwise, just click the `Select All` button to select all Default patches.

> [!IMPORTANT]
> For ROOT YouTube / YT Music installations, the `GmsCore support` patch must be excluded. In non-ROOT environments the patch will be hidden and included automatically.

5. If you did not upload an APK in step 3, a menu will appear where you can choose the version of the app to patch. Select the first option, marked `(AUTO SELECTION)`, or select a version marked as `(suggested)`. After the APK is downloaded, click `Continue` and wait for patching to complete.

6. For non-ROOT installations, the patched APK will be saved to your device and it must be manually installed. The path to the APK will be displayed at the bottom of the patch log. For ROOT installations, the app will be mounted automatically.


Additional info
==

### Updating rvx-builder:

To update rvx-builder, run either of these commands in Termux:
```
rvxup
```
or
```
./rvx-builder.sh update && ./rvx-builder.sh run
```

### Reinstalling rvx-builder:

To reinstall rvx-builder, run either of these commands in Termux:
```
rvxre
```
or
```
./rvx-builder.sh reinstall && ./rvx-builder.sh run
```

Troubleshooting
==
**1. If encountering an error when installing rvx-builder for the first time:**

- Ensure that Termux is not the Play Store version of Termux
- Try reinstalling Termux
- Try changing networks, disable VPN and adblockers, etc.
- Try entering the following command:
```
apt-get autoremove nodejs-lts -y && pkg install nodejs-lts -y && apt-get autoremove openjdk-17 -y && pkg install openjdk-17 -y && ./rvx-builder.sh run
```

**2. If rvx-builder worked in the past, but an issue occurred when using it again:**

- Try reinstalling rvx-builder with the following command:
```
./rvx-builder.sh reinstall && ./rvx-builder.sh run
```
or
```
rvxre
```

**3. If an issue occurs during the patching process:**

- Ensure that Termux has battery optimization exclusions
- Reinstall rvx-builder with the following command:
```
./rvx-builder.sh reinstall && ./rvx-builder.sh run
```
or
```
rvxre
```

___
- If you encounter any other issues, please report them on the [GitHub issues page](https://github.com/inotia00/rvx-builder/issues).