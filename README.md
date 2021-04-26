# NadeTails
## What is NadeTails?

NadeTails give you the advantage of tracing your projectiles (smokes, molotovs, grenades or flashbangs), so you can see where they land. This can enhance your practice routines, and even enhance your game!

## How does it work?

It's fairly a plug-and-play plugin! You will be generated a CFG file, that you use to customize your tail.

### Installation

All you need is to download the release on the right, and you are ready to go. You can of course look down under here for ConVars.

### ConVars

* g_Enabled - Enables Nade Tails (0/1). (Default: 1)
* g_AllowPlayers - Allow players to use nade tails with !tails, otherwise admins only (0/1) (Default: 1)
* g_DefaultAlpha - Default alpha for trails, all predefined colors will use this alpha (0 is invisible, 255 is solid). (Default: 255)
* g_DefaultOn - Tails on for all users, Set to 0 to require user to type !tails to use (Default: 1)
* g_EnableHETails - Enables Nade Tails on HE Grenades (0/1). (Default: 1)
* g_EnableFlashTails - Enables Nade Tails on Flashbangs (0/1). (Default: 1)
* g_EnableSmokeTails - Enables Nade Tails on Smoke Grenades (0/1). (Default: 1)
* g_EnableDecoyTails - Enables Nade Tails on Decoy Grenades (0/1). (Default: 1)
* g_EnableMolotovTails - Enables Nade Tails on Molotovs (0/1). (Default: 1)
* g_EnableIncTails[ - Enables Nade Tails on Incendiary Grenades (0/1). (Default: 1)
* g_HEColor - Tail color on HE Grenades. (Default: random)
* g_FlashColor - Tail color on Flashbangs. (Default: random)
* g_SmokeColor - Tail color on Smoke Grenades. (Default: random)
* g_DecoyColor - Tail color on Decoy Grenades. (Default: random)
* g_MolotovColor - Tail color on Molotovs. (Default: random)
* g_IncColor - Tail color on Incendiary Grenades. (Default: random)
* g_TailTime - Time the tail stays visible. (Default: 20.0)
* g_TailFadeTime - Time for tail to fade over. (Default: 1)
* g_TailWidth - Width of the tail. (Default 1.0)

It is recomended you edit these ConVars inside csgo/cfg/sourcemod/plugin.NadeTails.cfg (which is created on first run) otherwise you might have some issues with your settings saving.

### Commands

* tails - Toggles grenade tails.
* tailsmenu - Admin menu to toggle Nade Tails on players (Flag required: ADMFLAG_KICK or override using https://wiki.alliedmods.net/Overridi...ess_(SourceMod)

### Colors

Colors for the trails can be set in two different ways, using predefined colors, or manually defined RGB(A) values. (Alpha is optional).
The predefined colors are:

* Black
* White
* Red
* Lime
* Blue
* Yellow
* Cyan / Aqua
* Magenta / Fuchsia
* Silver
* Gray
* Maroon
* Olive
* Green
* Purple
* Teal
* Navy

Manually defined colors are passed as RGBA strings.

**Color Examples:**
* sm_tails_hecolor "red"
* sm_tails_flashcolor "white"
* sm_tails_decoycolor "0 0 128 255" //RED GREEN BLUE ALPHA
* sm_tails_smokecolor "0 255 255" //this defaults the alpha to 225
* sm_tails_inccolor "random" //chooses random color

You can find a preview [here](https://i.imgur.com/MJXEcna.png)

## Note About The Current State

This plugin is an old plugin, that I have decided to revive. The reason is, that we (Esport Harte, a CS:GO union I play in) use this plugin a lot, and we really needed it to work properly.

## Changelog

*ChangeLog:
Version 1.0:*
* *Initial Release*

*Version 2.0:*
* *Added Convars for everything ever (colors, time, invididual enable, etc..)*
* *Added a menu to toggle tails on clients*

*Version 3.0:*
* *Fixed small FCVAR problems*
* *Fixed a problem with EdictClass not being correct and causin an error*
* *H3Bus added **a** flag to also respond to NadeTails. This means that if you have VIP flagged **a** they can do this also.*

**Current Version: 3.0**

## Credits

- Internet Bully - Original creator of the project.
- @kstheman - Reforger of the project.
- H3Bus - Making **a** available as a flag to use the plugin for VIP members.


## To-Do

*There will eventually be added some things:

* Translations
* Fixes and repairs*

## Links

SourceMod - https://forums.alliedmods.net/showthread.php?t=240668

