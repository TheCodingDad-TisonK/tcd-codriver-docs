# FAQ

## Do I need to install another plugin first?

No. The download already contains the open-source hry-core framework the plugin runs on. Install the files from the zip and you are done.

## Which keys does the plugin use?

`Delete` opens and closes the TCD Co-Driver window and gives you the mouse. `F7` shows or hides the HUD. hry-core's own menu is hidden, so to change the keys edit the keybinds file in the hry-core folder under `%LOCALAPPDATA%`.

## The website shows a "You are about to visit" warning page

The public site is served through a free ngrok tunnel. ngrok shows that anti-abuse page **once per browser per 7 days**. Click **Visit Site** to continue; it will not appear again for a week. The plugin's own license checks are not affected.

## Windows says "Windows protected your PC"

The plugin is not digitally signed yet. If you downloaded the zip from your account page, choose **More info → Run anyway**. You can verify the file with the SHA-256 shown on your account page.

## Can I use it online or on a multiplayer server?

It has not been tested with multiplayer services. The plugin only reads data the game shares with plugins and does not change gameplay, but check the rules of the service you play on before using any plugin.

## Does it change the game?

No. It does not add trucks, maps or cheats, and does not alter how the game plays. It reads telemetry and draws it back to you.

## Does the coach send my driving data anywhere?

No. Scores, settings and the logbook stay on your computer in `%LOCALAPPDATA%\TcdCoDriver`. The license check only sends your key and computer identifier to the license server.

## The game asks about "advanced SDK features" — should I allow it?

Yes. Choose **Yes** once when the game asks, otherwise plugins cannot read telemetry.

## The window opens but the mouse does not work

Press `Delete` again. The overlay gives you the mouse while the window is open; game keys do not work while it is open.

## The plugin says my license cannot reach the server

The server may be briefly unavailable. A working license keeps going offline for up to a week. Check the website later and use the **Re-check** button on the License tab.

## Where do I send a bug report?

Use the contact form on the website and include the end of `Documents\hry_core\ets2\hry_core.log` (or `...\ats\hry_core.log`).
