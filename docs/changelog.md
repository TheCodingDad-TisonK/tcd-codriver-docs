# Changelog

> **Where things live:** the public overview and prices are on the [landing page](https://thecodingdad-tisonk.github.io/tcd-codriver/), accounts and keys are on the license site linked there, and these guides are in [this repo](https://github.com/TheCodingDad-TisonK/tcd-codriver-docs).

## 0.3.0 (26 Nov 2026)

- **A HUD that follows your job**: on a delivery the main panel shows the destination with the distance and time to go and a deadline chip, the cargo condition and the fuel; on an ETS2 Coaches DLC job it shows the next stop with its arrival time and a late or on-schedule chip, the passengers' rating live and your on-time score. The speed and the limit sign appear only while you are over the limit. With no job the classic speedometer HUD is shown. Each job HUD can be turned off in Settings
- **No turn signals on the HUD**: the cab already shows them
- **ETS2 Coaches DLC job fixed**: the stop details now reach the plugin. hry-core already held the game's job events, so the plugin never received them; hry-core now passes them on. The `hry-core.dll` in the zip is required (`Install.bat` copies it)
- **Coach job card**: a timetable with planned and actual times, delays, boarding and alighting and the current stage marked; bus lines of up to 64 stages (the old limit was 16)
- **Punctuality score** from the actual arrival times, a chart of the passengers' rating over the job, and status chips (tour or bus line, on time, running late, passengers on board)
- **Coach hints**: behind the timetable, passengers feeling hard driving, a falling rating. The HUD shows a short late hint. Rest hints stay quiet during a coach job
- **Coach jobs in the logbook**: saved as a Coach tour or a Bus line with the passengers' rating, punctuality, passengers carried, the income the game expected and the planned distance; the CSV export and the Statistics tab have the coach columns and totals. A bus does not count in the truck fuel average or the most economical record
- **Coach summary**: after a coach job a card compares what it paid with what the game expected, and the distance driven with the planned one. The last coach job stays on the Dashboard until the next one starts
- Only the first job after the game starts is marked as a partial trip (every later job was marked by mistake)
- Game times are shown as a time of day instead of raw game minutes
- Coming next: calibrated coach score thresholds, after real-drive testing

## 0.2.0 (25 Nov 2026)

- **ETS2 Coaches DLC**: passenger satisfaction, stage and stop details, timetable, boarding/alighting counts and expected income on the Dashboard; a coach job loaded from a mid-job save is detected from live telemetry when the game does not send its config
- **Dashboard**: instruments (AdBlue, brake temperature, air pressure, oil, water, battery), in-game clock, vehicle identity, derived G indicator and connected-trailer readouts
- **Logbook**: trip reports show partial trips, autopark/autoload shortcuts and the currency of each game
- **Settings**: every option explained in the file itself, a `.bak` copy is kept, and failed file writes are reported on the About tab
- **Menu**: new Changelog tab; the website link on the About tab is now clickable
- Coming next: calibrated coach score thresholds and bus-job settlements in the logbook after real-drive testing

## 0.1.0 (first version)

- **Heads-up display**: speed, limit, gear, rpm with an economy zone, fuel, status chips, a coach strip, a trip score badge, a route line and a summary card after each delivery
- **Dashboard**: truck condition, current job, a two-minute speed chart, a coach summary and your latest deliveries
- **Driving coach**: scores each trip for economy, safety and smoothness, with ranked tips (limits are first estimates)
- **Logbook**: search and sort, a full report for each delivery, statistics and CSV export
- **License**: free 14-day trial, then a subscription; the plugin works offline for up to a week between check-ins
