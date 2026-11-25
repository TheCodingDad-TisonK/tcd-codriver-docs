# Installation

TCD Co-Driver 0.1.0 — about two minutes.

## What you need

- Euro Truck Simulator 2 or American Truck Simulator on Windows
- A license key. Create an account on the website and confirm your email to get a free 14-day trial key.

## Steps

1. Close the game.
2. Download the zip from your account page on the website and extract it anywhere (right-click → Extract All). Do not run `Install.bat` from inside the zip.
3. Double-click `Install.bat`. It looks for your game and asks before copying anything. Answer `Y` for the game you want.
4. Start the game. The first time, the game asks once whether to allow the plugin to use "advanced SDK features". Choose **Yes**.
5. In the game press **Delete**. The TCD Co-Driver window opens. Go to **License**, paste your key and press **Activate**.

## Windows warning

Windows may show "Windows protected your PC" because the plugin is not digitally signed yet. If you downloaded the zip from your account page, choose **More info**, then **Run anyway**. To check that the download is genuine, compare its SHA-256 hash with the one shown on your account page:

```powershell
Get-FileHash <the zip file>
```

## Manual install

If `Install.bat` does not find your game, it asks for the game folder — the one that contains the folder `bin`. To install by hand, copy everything inside `files\bin\win_x64\plugins` into:

```
<game folder>\bin\win_x64\plugins
```

Create the `plugins` folder if it is not there. You can install into both games; `Install.bat` asks once for each game it finds.

## Keys

| Key | What it does |
|---|---|
| `Delete` | Opens and closes the TCD Co-Driver window (and gives you the mouse; game keys do not work while it is open) |
| `F7` | Shows or hides the HUD |

The plugin runs on the open-source hry-core framework, which is included in the download. You do not need to install it separately. Its own menu is hidden; the keys can be changed in the keybinds file in the hry-core folder under `%LOCALAPPDATA%`.

## Uninstalling

Run `Uninstall.bat` from the extracted folder. It removes only `tcd-codriver.dll`. `hry-core.dll` and `hry_assets` are left in place in case another plugin uses them; remove them yourself if nothing else does.
