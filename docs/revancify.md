## About Revancify
Revancify is a tool for building ReVanced on termux

The developer of Revancify is [@decipher3114](https://github.com/decipher3114), visit the [Revancify repository](https://github.com/decipher3114/Revancify) for more info

#### How to install Revancify for the first time
1. Firstly, you have to install Termux. To do this, you have to install [F-Droid](https://f-droid.org/packages/com.termux/).

2. After that, you have to run these commands:

```
pkg update -y && pkg install git -y && git clone https://github.com/decipher3114/Revancify.git && ./Revancify/revancify
```

#### Usage
After installation, type `revancify` in termux and press enter.  
   
Or use with arguments. Check them with `revancify -h` or `revancify --help`  


## Guide with screenshots
0. If you are installing Revancify for the first time, you can select the source

![1](https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_1.png)

Select `inotia00`

1. Select `4 Update Resources` to download the latest patch

![2](https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_2.png)

2. You can select patches to include or exclude through `2 Select Patches`.

![3](https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_3.png)

If you are patching in a ROOT environment, you should exclude the `GmsCore support` patch.

If you are patching in a NON-ROOT environment, you should include the `GmsCore support` patch.

![4](https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_4.png)

3. Before starting the patch, Please read this [documentation]( https://github.com/inotia00/revanced-documentation/wiki/Before-start-(Prerequisites)#common)

4. Select `1 Patch App`

![5](https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_5.png)

From the Version Selection Menu, choose the version labeled '[RECOMMENDED]'.

![6](https://github.com/inotia00/revanced-documentation/blob/main/images/revancify_6.png)

The patch will automatically proceed and be installed on your device.