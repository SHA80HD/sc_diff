# Legal
This site is not endorsed by or affiliated with the Cloud Imperium or Roberts Space Industries group of companies. All game content and materials are copyright Cloud Imperium Rights LLC and Cloud Imperium Rights Ltd.. Star Citizen®, Squadron 42®, Roberts Space Industries®, and Cloud Imperium® are registered trademarks of Cloud Imperium Rights LLC. All rights reserved.

# Viewing Diffs
GitHub limits diff sizes on the website. You have to use an external application to view the full diff.

The different realms are split into individual branches.

## GitHub Desktop
You can use [GitHub Desktop](https://desktop.github.com/) to view the differences between patches.

![GitHubDesktop](https://github.com/SHA80HD/sc_diff/assets/148783655/fdc2e5b5-a712-4b74-9006-7e565b8cd29c)

## WinMerge
[WinMerge](https://winmerge.org/?lang=en) is great also but requires you to download two sets of data.

# How To Extract Files Yourself

## unp4k

1. Download and unzip: [unp4k](https://github.com/dolkensp/unp4k/releases/tag/v3.13.21)
2. From a command prompt: `unp4k.exe "c:\Program Files\Roberts Space Industries\StarCitizen\LIVE\data.p4k" *.xml`
    - If you want all files AND assets, remove `*.xml`. This takes much longer to unpack and unforge.
    - Switch LIVE to PTU or EPTU to unpack those realms.
    - Create separate folders for different builds if you want to diff them later.
3. From a command prompt: `unforge.exe Data`
4. From a command prompt: `unforge.exe Engine`
5. View files with text editor of your choice.
    - [VS Code](https://code.visualstudio.com/)
    - [WinMerge](https://winmerge.org/?lang=en)

## Starfab (Highly Recommended)

1. Download and install [Starfab](https://gitlab.com/scmodding/tools/starfab/-/releases)
2. Run it

## Interesting Directories To Look At To Get Started

- Actor
    - Data\Libs\Foundry\Records\actorhealthcomponent
    - Data\Libs\Foundry\Records\actorstatuscomponent
    - Data\Libs\Foundry\Records\damage
    - Data\Libs\Foundry\Records\entities\scitem\characters\human\armor\pu_armor

- FPS Weapons and Ammo
    - Data\Libs\Foundry\Records\ammoparams
    - Data\Libs\Foundry\Records\entities\scitem\weapons\fps_weapons
    - Data\Libs\Foundry\Records\entities\scitem\weapons\magazines

- Ships and Components
    - Data\Libs\Foundry\Records\entities\scitem\vehicles
    - Data\Libs\Foundry\Records\entities\scitem\weapons
    - Data\Libs\Foundry\Records\entities\scitem\ships
    - Data\Libs\Foundry\Records\entities\scitem\ships\weapons
    - Data\Libs\Foundry\Records\entities\spaceships
    - Data\Scripts\Entities\Implmentations
