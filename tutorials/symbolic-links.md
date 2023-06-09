---
description: Store your games in a different folder
---

# Symbolic links

Using Symbolic links is a solution provided natively in Windows that allows you point a logical folder to a folder stored on another place on your computer.

How is this interesting for ProjectArcade ?

The whole point of this feature is to allow you to physically store your roms in a different place than the standard \ProjectArcade\roms\ folder, for example you could store them on a separate Hard Drive which has a bigger storage size.

**Example:**

<figure><img src="https://i.imgur.com/xDr4OsT.png" alt=""><figcaption></figcaption></figure>

## Creating a symbolic link

To create a symbolic link in Windows, you can either use command lines in the console, or use a tool called "Link Shell Extension". The method described hereafter is the method with usage of this tool.

### Download Link Shell Extension

The program can be downloaded from the following website : [https://schinagl.priv.at/nt/hardlinkshellext/linkshellextension.html#download](https://schinagl.priv.at/nt/hardlinkshellext/linkshellextension.html#download)

### Use Link Shell Extension

Once installed, you need to reboot your computer or to close and restart the "explorer.exe" process.

Once done, new options will appear in the right-click context menu:

* Pick Link Source

<figure><img src="https://i.imgur.com/i6NrZGJ.png" alt=""><figcaption></figcaption></figure>

* Drop As...

<figure><img src="https://i.imgur.com/TMwcODp.png" alt=""><figcaption></figcaption></figure>

### Create a symbolic link with Link Shell Extension

In the next example, we will suppose that you are storing your 3do game ROMs in `D:\ProjectArcade\3do` and that you ProjectArcade installation folder is `C:\ProjectArcade`.

1. Ensure all your roms are properly copied to `D:\ProjectArcade\3do` and that your `C:\ProjectArcade\roms\3do` does not contain any important data you need to keep
2. Delete the `C:\ProjectArcade\roms\3do` folder
3. Right-click on the `D:\ProjectArcade\3do` folder and select "**Pick Link Source**"
4. Go to the `C:\ProjectArcade\roms` folder, right-click anywhere inside the folder and select "**Drop As... > Symbolic Link**"
5. Your `C:\ProjectArcade\roms` folder will now show a 3do folder icon with a small arrow ![](<../.gitbook/assets/image (6).png>)&#x20;

**Congratulations!** You have just created a symbolic link !

You can now repeat this operation for any folder that you would want to store in another place as the default one.



### Create a symbolic link with native Windows command

Let's use the same example as before and try to perform the Symlink creation manually.

1. sure all your roms are properly copied to `D:\ProjectArcade\3do` and that your `C:\ProjectArcade\roms\3do` does not contain any important data you need to keep
2. Delete the `C:\ProjectArcade\roms\3do` folder
3. Open Windows command and type the following command: `mklink /D "C:\ProjectArcade\roms\3do" "D:\ProjectArcade\3do`
4. Your `C:\ProjectArcade\roms` folder will now show a 3do folder icon with a small arrow ![](<../.gitbook/assets/image (6).png>)&#x20;

<figure><img src="https://i.imgur.com/wgrK31v.png" alt=""><figcaption></figcaption></figure>
