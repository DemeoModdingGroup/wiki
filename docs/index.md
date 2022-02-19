# Demeo Modding Wiki
Please note that this wiki is still in development and may not be complete in some sections. Pardon our mess.

## Compatibility of Mods
In order to ensure compatibility of mods across Demeo the modding community has selected specific utilities for use in developing and loading of mods.

## MelonLoader
[LavaGang](https://melonwiki.xyz/#/credits), the MelonLoader developers, have been working directly with Resolution Games to add somewhat of an official modding API to Demeo. All of these features are in the `Boardgame.ModdingAPI` namespace with the main feature being the mod menu which shows what mods you have installed.\

![screenshot of the mod menu](https://i.joezwet.dev/demeo-mod-menu.png)\

### Supported Platforms
This mod loader supports the PC VR client on both Oculus and Steam services.

### Installing MelonLoader

### Get MelonLoader
The Melon Loader developers have provided an easy to use installer and it is recommended to use the [MelonLoader.Installer.exe](https://github.com/LavaGang/MelonLoader/releases/download/v0.5.3/MelonLoader.Installer.exe).\
If you wish to use another install method you can find the other downloads here: It is recommended to use the That you can download here: [Melon Loader releases tab](https://github.com/LavaGang/MelonLoader/releases).\

???+ info
    Please note that this guide is for the Melon Loader `v0.4.1+` builds of Melon Loader. Check out the Official Melon Loader install guide if you need further assistance [here](https://melonwiki.xyz/#/README?id=automated-installation).

### Setup MelonLoader
You will need to execute the [MelonLoader.Installer.exe](https://github.com/LavaGang/MelonLoader/releases/download/v0.5.3/MelonLoader.Installer.exe) from your 'Downloads' folder, you may encounter a Windows Security or Anti-Virus alert that you will need to by-pass in order to run the installer.\
![MelonLoader Automated Install](https://i.joezwet.dev/hWD9lA8l0N.png)\
Once the installer is open you will need to browse to the location of the `demeo.exe` to begin the MelonLoader install. Please 'Select' and navigate to your Demeo installation.

**Typical Install Locations**
Steam Default location:
```
C:\Program Files\Steam\steamapps\common\demeo\
```
Oculus Default location:
```
C:\Program Files\Oculus\Software\Software\resolution-games-demeo\
```

You would repeat the process to Uninstall MelonLoader choosing 'Uninstall' instead of 'Install'.

## Getting an Alpha build (optional)
Now that you have the base loader installed you may need to install the latest alpha build from the Melon Loader [Actions tab](https://github.com/LavaGang/MelonLoader/actions).\
Click on the latest run and download the artifact labeled `MelonLoader.x64.CI`.\
Extract the zip so that `version.dll` is in the same folder as `demeo.exe`.
