# Customize Mega-Bezels

ProjectArcade allows you to download Duimon's Mega-Bezel pack (you can find more information in the [Decorations & Bezels](../advanced-features/decorations-and-bezels.md#mega-bezels) section of the wiki).

This page will give you details and one example showing you how it is possible to customize the Mega-Bezels.

## Location of all required files

First, you need to understand where the files we will be modifying are located.

### ProjectArcade files

Files used by the ProjectArcade interface to display the list of available Mega-Bezels are located in the `system\shaders\configs` folder of your ProjectArcade installation.

<figure><img src="https://i.imgur.com/7SEscUi.png" alt=""><figcaption></figcaption></figure>

Each subfolder contains a `rendering-defaults.yml` file specifying:

\- the system concerned,\
\- the "preset" that is applied for this system.

<figure><img src="https://i.imgur.com/tLGT8CN.png" alt=""><figcaption></figcaption></figure>

### Retroarch

Files that are used in Retroarch to enable Mega-Bezels are stored in the `emulators\retroarch\shaders\shaders_slang\Duimon-Mega-Bezel\` folder of your ProjectArcade installation.

<figure><img src="https://i.imgur.com/fgpBn8a.png" alt=""><figcaption></figcaption></figure>

## Adding a new Mega-Bezel Preset entry to ProjectArcade

### Step 1 : preset customization

In the example we will use for this tutorial, we will add a new preset to the Saturn system that will mirror the bezel image so that it appears in the correct direction (default bezel might be flipped on some systems).

<figure><img src="https://i.imgur.com/c0QPInK.png" alt=""><figcaption><p>Example of "mirrored" bezel for Saturn (see the text on the top right)</p></figcaption></figure>

Let's start by copying the existing preset files and customize them by adding the instruction to mirror the bezel.\
First, we will need to copy the existing presets located in the `emulators\retroarch\shaders\shaders_slang\Duimon-Mega-Bezel\` folder.

We will copy the ones that are the most used for the SATURN system, \[Bezel] and \[Bezel]-\[Night] (advanced versions):

<figure><img src="https://i.imgur.com/INWfURU.png" alt=""><figcaption></figcaption></figure>

Then, we will rename the presets with a name that will help us identify them later.

Let's add the \[VFlip] tag (as Vertical Flip), and ensure we do not add any blank space in the name:

<figure><img src="https://i.imgur.com/VJea3ZI.png" alt=""><figcaption></figcaption></figure>

Next, we will open both files with a text editor and add the instruction to flip the image:

`HSM_FLIP_VIEWPORT_VERTICAL = "1.000000"`

<figure><img src="https://i.imgur.com/HiXJkq0.png" alt=""><figcaption><p>The lines in this file are the instructions given to RetroArch for displaying correctly the effects.</p></figcaption></figure>

### Adding the new preset to the ProjectArcade menu

Go to the folder `system\shaders\configs` and copy one of the existing subfolders (in our example "mega-bezel-advanced-night"), rename the new folder "mega-bezel-advanced-night-VFlip" (this is the name that will appear in the ProjectArcade menu :

<figure><img src="https://i.imgur.com/AxSDahs.jpg" alt=""><figcaption></figcaption></figure>

Inside the modified folder, open the file named "rendering-defaults.yml" (This is the file telling RetroArch what preset to use for a system).

The first line corresponds to the system, as known by ProjectArcade (use the official system name that can be found in the `\emulationstation.emulationstation\es_systems.cfg` file).

The second line indicates the preset to use for this system by pointing to the .slangp file (relative path is used here) :&#x20;

<figure><img src="https://i.imgur.com/SvVwEBZ.png" alt=""><figcaption></figcaption></figure>

In our example, we will use the preset we have modified (note that the extension is not needed):&#x20;

<figure><img src="https://i.imgur.com/nOO5d9c.png" alt=""><figcaption></figcaption></figure>

Save, and close the file.



In ProjectArcade, the new entry "mega-bezel-advanced-night-vflip" is now available in the shaders section.

<figure><img src="https://i.imgur.com/r6R365E.png" alt=""><figcaption></figcaption></figure>

The Mega-Bezel is now displayed in the correct way.

<figure><img src="https://i.imgur.com/EkippyM.png" alt=""><figcaption></figcaption></figure>

Many more settings are availabe, and each system has multiple presets.\
You can refer to Duimon's Github page for more information : [https://github.com/Duimon/Duimon-Mega-Bezel](https://github.com/Duimon/Duimon-Mega-Bezel)

{% embed url="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FCgoewyw8Sagl6SNUMrCG%2Fuploads%2F4GBUEMCfoEYBAeER58HG%2FEdit%20Shaders%20Presets.mp4?alt=media&token=ae36a62c-76b7-4e24-a0b3-86581f79cba9" %}
