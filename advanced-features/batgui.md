# Batgui

BatGui is a software provided by RetroBat team for ProjectArcade and available at the root of your ProjectArcade folder

<figure><img src="https://i.imgur.com/NRJN9Ju.png" alt=""><figcaption><p>BatGui.exe</p></figcaption></figure>

**The tool allows you to:**

* Help managing [projectarcade.ini](projectarcade.ini.md) config file
* Manage System List
* Edit Gamelists (update game metadata)
* Generate windows game .bat files for [Steam ](../systems-and-emulators/supported-game-systems/others/windows.md#adding-a-steam-game)games from your library
* Generate .m3u file for [Xbox 360 ](../systems-and-emulators/supported-game-systems/game-consoles/microsoft-consoles/xbox-360.md#adding-xbla-xbox-live-arcade-games)and [PS3 ](../systems-and-emulators/supported-game-systems/game-consoles/sony/playstation-3.md#adding-ps3-games)emulators
* Convert iso/cue format into CHD format
* Change the version of the SDL library and reset controller configuration



<figure><img src="https://i.imgur.com/5xMsnHr.png" alt=""><figcaption></figcaption></figure>

### ProjectArcade ini

With BatGui.exe, you can edit the settings of your projectarcade.ini file

<figure><img src="https://i.imgur.com/bQBN1Ux.png" alt=""><figcaption></figcaption></figure>

### System list

In this menu it is possible to update `es_systems.cfg` file, for example it is possible to remove an extension for a system.

<figure><img src="https://i.imgur.com/HfiG9lD.png" alt=""><figcaption></figcaption></figure>

### Gamelist editor

In this menu it is possible to update `gamelist.xml` file for a system, metadata of individual games can be updated here as well as medias of games.

<figure><img src="https://i.imgur.com/Mjir7uB.png" alt=""><figcaption></figcaption></figure>

### Add Steam Library

In this menu it is possible to generate automatically the .bat file in your `\roms\windows` folder in order to [add your Steam games to ProjectArcade](../systems-and-emulators/supported-game-systems/others/windows.md#adding-a-steam-game).

<figure><img src="https://i.imgur.com/w4IotL3.png" alt=""><figcaption></figcaption></figure>

### M3U Creator

In this menu it is possible to generate automatically the .m3u file in your [`\roms\ps3`](../systems-and-emulators/supported-game-systems/game-consoles/sony/playstation-3.md#adding-ps3-games) or [`\roms\xbox360`](../systems-and-emulators/supported-game-systems/game-consoles/microsoft-consoles/xbox-360.md#adding-xbla-xbox-live-arcade-games) folders for games installed in the emulator.

<figure><img src="https://i.imgur.com/cs7oKVW.png" alt=""><figcaption></figcaption></figure>

### CHD Manager

In this menu it is possible to convert a ISO/CUE rom format into CHD format for emulators that support CHD format.

<figure><img src="https://i.imgur.com/B9Qz6bc.png" alt=""><figcaption></figcaption></figure>

### Change SDL library version and reset controller configuration

The "SDL Library Selector" menu allows you to reset controller configuration. This might be useful in case of conflict in the controller configuration module.\
Just click the "Reset GamePad config" button, all controller configuration will be deleted (except keyboard), and ProjectArcade will prompt you to configure your controller(s) again.\
Thie action performs a reinitialization of the **es\_input.cfg** file located in the `emulationstation\.emulationstation` folder of your ProjectArcade installation.

<figure><img src="https://i.imgur.com/uHLuZaf.png" alt=""><figcaption></figcaption></figure>

From the "SDL Library Selector" menu, you will also be able to choose between different SDL versions. This option might be useful if some of your controllers are not correctly recognized as a last resort option (always start from the more recent, and try the versions from the most recent to the oldest).\
To do so, choose a DLL from the dropdown list, and click "Close". Then click "Reset GamePad config". You can now start ProjectArcade and reconfigure your controller.

<figure><img src="https://i.imgur.com/tw0aDbr.png" alt=""><figcaption></figcaption></figure>
