How to install rvx-builder for the first time
==
1. Firstly, you have to install Termux. To do this, you have to install [F-Droid](https://f-droid.org/packages/com.termux/).

2. After that, you have to run these commands:

```
curl -sLo rvx-builder.sh https://raw.githubusercontent.com/inotia00/rvx-builder/revanced-extended/android-interface.sh && chmod +x rvx-builder.sh && ./rvx-builder.sh
```

※ If an error occurs, enter it line by line: 
```
curl -sLo rvx-builder.sh https://raw.githubusercontent.com/inotia00/rvx-builder/revanced-extended/android-interface.sh
```
```
chmod +x rvx-builder.sh
```
```
./rvx-builder.sh
```

※ During initial installation, termux will ask if you want to update additional packages. (Enter Y or N.)

3. After installing, `rvx-builder` will run automatically!

Run command
==
When to run rvx-builder in termux, just type these commands:
```
./rvx-builder.sh run
```
or
```
rvx
```

Update command
==
If there is an update of rvx-builder, just type these commands:
```
./rvx-builder.sh update && ./rvx-builder.sh run
```
or
```
rvxup
```

Reinstall command
==
When an issue occurs so you need to reinstall rvx-builder, just type these commands:
```
./rvx-builder.sh reinstall && ./rvx-builder.sh run
```
or
```
rvxre
```

Troubleshooting
==
1. If you get an error when installing rvx-builder for the first time
- Check if termux is downloaded from [F-Droid](https://f-droid.org/packages/com.termux/).
- Try reinstalling termux
- Try changing vpn/dns
- Try entering the following command:
```
apt-get autoremove nodejs-lts -y && pkg install nodejs-lts -y && apt-get autoremove openjdk-17 -y && pkg install openjdk-17 -y && ./rvx-builder.sh run
```

2. If you used rvx-builder without issues before, but the issue occurred while using it again
- reinstall rvx-builder:
```
./rvx-builder.sh reinstall && ./rvx-builder.sh run
```

3. If an issue occurs during the patching process
- Read the [Common document](https://github.com/inotia00/revanced-documentation/wiki/Before-start-(Prerequisites)#common) again.
- Make sure termux has battery optimization exclusions.
- Make sure your device has `arm64-v8a` architecture. (Probably, other architectures are not supported.)
- reinstall rvx-builder:
```
./rvx-builder.sh reinstall && ./rvx-builder.sh run
```
or
```
rvxre
```

※ If you encounter any other issues, please report them on the [github issues page](https://github.com/inotia00/rvx-builder/issues).