---
title: DSOne SDHC
---

![DSOne SDHC](../images/dsone.png){ align=right width="115"}
# DSOne SDHC
## supercard.sc

!!! info
    
    The DSOne SDHC is one of the SuperCard team's later flashcarts, with some uncommon features like RTS (Real Time Save), and an in-game menu. EvolutionOS, the flashcart's stock kernel, is compatible with nearly all DS games and romhacks, so it is fairly reliable.

    Unfortunately, some DSOne carts have faulty PSRAM, which causes EvolutionOS to not work on those carts due to EOS relying on the PSRAM to function. These carts can use YSMenu instead to retain basic DS game loading functionality, but will not have access to EvolutionOS-exclusive functionality like RTS.

### Setup Guide:

=== "Evolution OS"

    1. Format the SD card you are using by following [this guide.](https://wiki.hacks.guide/wiki/Formatting_an_SD_card)
    
    1. Download the [Evolution OS SP6 kernel.](https://archive.flashcarts.net/SuperCard/DSONE_SDHC_DSONEi/SuperCard_DSONE_SDHC_EOS_sp6_20121206.zip)
    
    1. Open/extract the zip file, and copy *the contents* into the root of your SD card.
    
    1. If you'd like to be able to use cheats on your games, download a [cheat database.](https://github.com/DeadSkullzJr/NDS-i-Cheat-Databases/releases/latest)
    
    1. You will need the `usrcheat.7z` file. Extract it using [7-Zip](https://www.7-zip.org/), inside you will find a `usrcheat.dat` file. Copy this file into the `_dsone` folder on your SD card.
    
    1. Create a `Games` folder in your SD card root, and place your `.nds` game ROMs inside. You can also create additional folders to help with organizing/categorizing your ROMs.
    
    1. Insert the SD card back into your cart, plug the cart into your DS, and see if it boots into the menu.

    !!! tip
        If you'd like to learn more about the various options and functionality found in EvolutionOS, check out the [DSOne Manual](https://github.com/Sanrax/DSOneManual)!

=== "YSMenu - Broken PSRAM Carts"
    
    1. Format the SD card you are using by following [this guide.](https://wiki.hacks.guide/wiki/Formatting_an_SD_card)
    
    1. Download the [RetroGameFan YSMenu 7.06 kernel.](https://gbatemp.net/download/retrogamefan-multi-cart-update.35737/download)
    
    1. Extract the YSMenu .7z file you downloaded using [7-Zip](https://www.7-zip.org/), then go into the `DSONEi SDHC YSMenu` folder.
    
    1. From this folder, copy the following files/folders to your SD card root:
    
        - `Games` folder
    
        - `TTMenu` folder
    
        - `SCFW.SC`
    
        - `TTMenu.dat`
    
    1. Place any `.nds` game ROMs you'd like to play into the `Games` folder.
    
    1. Insert the SD card back into your cart, plug the cart into your DS, and see if it boots into the menu.

=== "MultiMenuDS - Broken PSRAM Carts"

    !!! info

        MultiMenuDS is a kernel that provides an AKMenu/Wood style frontend while using the TTMenu game loader. It supports Acekard themes & cheats and is also able to make use of nds-bootstrap.

    1. Format the SD card you are using by following [this guide.](https://wiki.hacks.guide/wiki/Formatting_an_SD_card)

    1. Download the [MultiMenu DSOne SDHC Package.](https://github.com/coderkei/MultiMenuDS/releases/latest/download/DSOneiSDHC_MultiMenu.zip)

    1. Open/extract the zip file, and copy *the contents* into the root of your SD card.

    1. If you'd like to be able to use cheats on your games, download a [cheat database.](https://github.com/DeadSkullzJr/NDS-i-Cheat-Databases/releases/latest)

    1. You will need the `usrcheat.7z` file. Extract it using [7-Zip](https://www.7-zip.org/), inside you will find a `usrcheat.dat` file. Copy this file to `TTMenu/cheats/` on your SD card. (Create the `cheats` folder if it doesn't exist)

    1. Create a `Games` folder in your SD card root, and place your `.nds` game ROMs inside. You can also create additional folders to help with organizing/categorizing your ROMs.

    1. Insert the SD card back into your cart, plug the cart into your DS, and see if it boots into the menu.

    1. (Optional) Download the [nds-bootstrap package](https://github.com/DS-Homebrew/nds-bootstrap/releases/latest/download/nds-bootstrap.zip) and extract it. Copy `nds-bootstrap-release.nds` to the `_nds` folder on your SD card.

    !!! tip

        This kernel uses the TTMenu game loader which some ROM Hacks are not compatible with. If you get an error code when loading a ROM Hack, Follow Step 8 above. Afterwards highlight the game and press `Y` and then press `Y` again for Game Settings. Change option under `Use ROM loader` from `default` to `nds-bootstrap`. Press `A` to save.