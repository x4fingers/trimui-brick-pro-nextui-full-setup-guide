# TrimUI Brick Pro NextUI Full Setup Guide

## Install NextUI

### Requirements:

- SD card with minimum 64GB storage, U3 class (UHS Speed Class 3)
- SD card adapter or USB hub has SD Card reader.

### Installation guide

- [NextUI](https://github.com/LoveRetro/NextUI): do as they said and configure what ever you want.

## Install games

### Portmaster

If you need to play ported old PC games, you need install [Portmaster](https://portmaster.games) from **Pak Store > Emulators**.

Steps:

- Step 1: Download game patches directly from [Portmaster website](https://portmaster.games/games.html) or Portmaster app on your device.
- Step 2.1: If it was **Ready to run** games, nothing needs to be done.
- Step 2.2: If it was **File needed** games, you need to find game files yourself from Steam, GOG, or other sources.

#### Game download sources

For people who can't purchase to get **File needed** games's folder

| Source                                                                          | Description                                          |
| ------------------------------------------------------------------------------- | ---------------------------------------------------- |
| [Portmaster ports 202405](https://archive.org/download/portmaster_ports_202405) | Common Portmaster game files, last updated: May 2024 |
| Steam RIP                                                                       | A source for Steam game data files                   |
| GOG Unlocked                                                                    | A source for GOG game data files                     |
| FitGirl Repacks                                                                 | Current status: no accessible                        |

Note:

- Be patient. On first run, it shouldn't work because of different file structure of NextUI and this source not configured for NextUI.
- Only use official `.sh` file from Portmaster, don't use outdated `.sh` file from this download source, only take game files then copy to game data folder.
- Some patches required only Windows or Linux game data folder, read instructions carefully before download games.
- If you are not an advanced user (developer, OS/game builder, ...), an AI Agent (Claude Code, Codex, ...) may help you setup games correctly on SD card.

#### Recommended games

- GTA Vice City
- GTA 3
- Stardew Valley
- Half-Life

### PS, PSP and other platforms

Install required emulators from **Pak Store > Emulators**

By default, prebuilt emulators on NextUI can run almost games. But some game may required a BIOS file to make it work properly.

Steps:

1. Download games BIOS and ROM files.
2. Copy BIOS files to `Bios/<emualtor_name>` folder.
3. Copy ROM files to `Roms/<emualtor_name>` folder.

#### Game download sources

| Source                                                                                   | Description                                                                                              |
| ---------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| [Minimal set retro collection](https://archive.org/details/minimal-set-retro-collection) | Almost ready to run game you need here. I tested many games and it should work.                          |
| [TOPO game library](https://game.toposhop.vn)                                            | A library contributed by Vietnamese retro gamers community. Not all games will work but just try anyway. |

#### Recommended games

**Individual games**

- Slient Hill
- Spider-Man
- Tomb Rider
- Prince of Persia - The sands of time
- Resident Evil 2
- Rockman X
- Zombie Ate My Neighbors
- Tank 90

**Series**

- Contra series
- Bomberman series
- Megaman series
- Dragon Ball series
- Street Fighter series
- Pokemon series
- Super Mario series
- Harvest Moon series
- Final Fantasy series

## Install apps

I won't provide a guide for installing apps on NextUI. Because of 3 reasons:

- Installation was easy and won't take much time.
- Apps on retro handheld devices it hard to input, not easy to navigate and may require better hardware specs to use smoothly.
- Gaming devices are designed for gaming.

## Troubleshooting

### Known issues

| Issue                                                                                                                                            | Fix                                                                                                                       |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------- |
| Some Portmaster game should configured correct resolution for this device, otherwise game may not run properly. Example: GTA Vice City and GTA 3 | Edit `reVC.ini`/`re3.ini` file, change from `Width=640 Height=480` to `Width=1024 Height=768` to match device resolution. |
| Doom 3 can't start new game, freeze on loading screen. If disabled audio, game can start but will freeze again.                                  | No fix yet. Audio driver issue and performance isssue.                                                                    |
| Can't run Forager (only support Linux version up to v2.0.4, newer version deprecated)                                                            | No fix yet. TrimUI CFW doesn't has 32-bit ARM compability layer at OS level                                               |

### Unresolved issues

| Issue                                                                                                                                           | Fix                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------- |
| I haven't found the way to install [Retroarch](https://www.retroarch.com/) on NextUI yet, so I can't use it for game required `libretro` cores. | Waiting contribution... |

## Contributing

Contact me on [Telegram](https://t.me/x4fingers) to contribute or create PR.

Happy gaming!
