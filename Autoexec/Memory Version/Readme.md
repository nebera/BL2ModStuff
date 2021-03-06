# Available Settings explained
***patchname=patch.txt***

Patchfilename to autoexec

***delay=8000***

Delay to wait before autoexec the patch. To make sure everything is properly loaded before executing.

***RapidFireDelay=20***

Delay between clicks for the rapidfire-script. Using the script is not really recommended though.

***Hexedited=False***
Use ***False*** if you haven't hex-edited your Borderlands2.exe. This will temporarily patch the game when it's running.

***Bypass=False***
Set Bypass to ***True*** if you want to enable the Sanity-Check-Bypass.

## Differences to the normal version
This is basically just an alternative version.
This one doesn't rely on finding the specific image anymore. Instead it reads the game processes memory to determine whether you're in the menu or not.

This makes it a lot more reliable if you're not using launch-options that skip the Startupmovies for example.

It's basically working the same way as the LiveSplit-Plugin that speedrunners use.

I've been trying to find a way to also determine whether the console is currently open or not. It basically works the same way. This also doesn't rely on finding specific pixels/images anymore.

## Functions
1. Renaming the exe to ***Launcher.exe*** and putting it into the ***Win32*** folder (rename the default Launcher.exe, JIC) will allow you to run the Autoexec-Tool even if you launch the game over steam directly. Thanks to Magic_Gonads for the idea.
2. Automatic temporarily "hexediting" the Borderlands2.exe. Based on Magic_Gonads idea and CE-Table. To use this, set ***Hexedited*** in the Autoexec.ini to ***False***

## Advantage
    * Should be a lot more reliable
## Disadvantage
Chances are, this won't happen anytime soon, if at all - 
    
    * It'll most likely break if there ever comes an update for BL2.

## Note
If you have used previous versions, you probably need to increase the delay in the ini-file. Increasing it by 1500-2000 should give you pretty much the same result as before.


# Changelog
- When using this as a replacement for ***Launcher.exe*** the Steam Launchparameters are now handeled automatically. No more need to add them to the INI-file.

-Added new functions to automate the temporary patching the CE-Table from Magic_Gonads has done.

This allows you to use the patches without haven to do any hex-editing. Thanks to Magic_Gonads for the idea and CE-Table :)

-Added the option to replace the Launcher.exe, which steam calls, even if you use the launchoption ***-NoLauncher*** 

To use it, just rename your old Launcher.exe and rename this scripts exe to ***Launcher.exe***. This script will check if its own name is ***Launcher.exe*** to decide to either run ***Borderlands2.exe*** or the steam-link.
