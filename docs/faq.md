# FAQ

> **Where things live:** the public overview and prices are on the [landing page](https://thecodingdad-tisonk.github.io/tcd-codriver/), accounts and keys are on the license site linked there, and these guides are in [this repo](https://github.com/TheCodingDad-TisonK/tcd-codriver-docs).

## What is the website for?

The [landing page](https://thecodingdad-tisonk.github.io/tcd-codriver/) is the public front door: it explains the plugin, shows screenshots and prices, and hosts the legal pages. It is static, so it stays online even when the license server is down. To get a key or log in you follow its buttons to the license site, which is the running server that handles accounts and keys.

## Does it support the ETS2 Coaches DLC?

Yes. During a coach job the Dashboard shows passenger satisfaction with a chart of how it developed, which stop you are on, the timetable with planned and actual times and delays, a punctuality score, boarding and alighting counts and the expected income. The HUD shows the next stop, the passengers' rating and your on-time score instead of the speedometer. When the job ends it is saved in the Logbook as a Coach tour or a Bus line, with the rating, punctuality and passengers. These coach job features are new in 0.3.0 and are being tuned. If you load a save that was already mid-job, the game may not send the full stop details; in that case the plugin still detects the coach job from live telemetry and shows satisfaction. Starting a coach job after launching ETS2 gives the full details.

## Why is there no speedometer on the HUD during a job?

The truck and the coach already have a speedometer and turn signals in the cab. While you are on a delivery or a coach job the HUD shows what the cab does not: where you are going, the deadline or the timetable, how the cargo or the passengers are doing, and the fuel. The speed and the limit sign appear only when you are over the limit. With no job you get the classic speedometer HUD. You can switch each job HUD off in Settings.

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

## The game asks about "advanced SDK features": should I allow it?

Yes. Choose **Yes** once when the game asks, otherwise plugins cannot read telemetry.

## The window opens but the mouse does not work

Press `Delete` again. The overlay gives you the mouse while the window is open; game keys do not work while it is open.

## The plugin says my license cannot reach the server

The server may be briefly unavailable. A working license keeps going offline for up to a week. Check the website later and use the **Re-check** button on the License tab.

## Where do I send a bug report?

Use the contact form on the website and include the end of `Documents\hry_core\ets2\hry_core.log` (or `...\ats\hry_core.log`).
