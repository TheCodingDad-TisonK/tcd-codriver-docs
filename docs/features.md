# Features

> **Where things live:** the public overview and prices are on the [landing page](https://thecodingdad-tisonk.github.io/tcd-codriver/), accounts and keys are on the license site linked there, and these guides are in [this repo](https://github.com/TheCodingDad-TisonK/tcd-codriver-docs).

## The HUD

Drawn inside the game window while you drive. The cab has its own speedometer and turn signals, so while you are on a job the main panel shows what the cab does not: where you are going and how you are doing. Some parts are always there:

- **Status chips**: lights, parking brake, cruise control, low fuel, oil, temperature, battery and air pressure, only when switched on
- **Coach strip**: one short hint when it matters (over the limit, time to rest, long idling, high revs)
- **Trip score**: a ring with your running score and grade for the current trip
- **Trip assistant**: one line with what you need to know about the rest of the trip (see below)
- **Event cards**: short cards at the side of the screen for a fine, a toll, a ferry or damage to the cargo, with what it cost
- **Summary card**: a card after each delivery with your score, net income and the top tip. When the truck has stopped it is a large card with the route you drove, the score, the money, how the trip compares with your last ten and the experience you earned

### On a delivery

- **Destination**: the city you are delivering to, the cargo, the distance and time to go, and a chip with the deadline (amber when less than an hour is left, red when you are late)
- **Cargo**: a ring with the condition of the cargo, which empties as it takes damage
- **Fuel**: litres and range, amber when the tank is getting low
- **Speed**: only while you are over the limit, as the limit sign, your speed and a warning that fade away again afterwards

### On an ETS2 Coaches DLC job

- **Next stop**: where the bus is going, when it should arrive, how many minutes that is, and a chip: on schedule, minutes late or minutes early
- **Rating**: a ring with the passengers' rating right now, and a small arrow when it is falling or rising
- **On time**: your punctuality score for the job so far
- **Speed**: only while you are over the limit, as on a delivery

### With no job

The classic panel: big speed digits (red when clearly over the limit, amber when slightly over), the limit sign, the gear, the rpm bar with the economy zone marked, and the fuel in litres with the range. When you have a job and the delivery HUD is switched off, a route line under it shows the distance to go, the time left and whether you are on time.

Every part can be switched off in Settings, and each job HUD has its own checkbox there ("On a delivery, show the destination, deadline and cargo" and "On a coach job, show the next stop and passenger rating").

### Make it yours

- **Themes**: Amber, Ocean, Forest, Crimson, Violet and Contrast. The theme colours the window and the HUD
- **Layout editor**: in Settings choose "Arrange the HUD", then drag each part where you want it and use the sliders to resize or hide it. "Reset the layout" puts everything back
- **Night dimming**: the HUD follows the in-game time and the headlights and gets a little dimmer and warmer after dusk
- **Profiles**: save the whole setup under a name and load it again later. A profile holds the look and the options, never your fuel price, income goal or anything else personal

## Trip assistant

Uses the deadline, the distance to go, your average speed on the trip, the game's rest timer and your fuel:

- **Arrive on time**: the average speed you need (distance divided by the time left) next to what you average. It says when you are on track and how much time you have to spare
- **Rest**: a rest that falls due before you arrive, and how long until it does
- **Fuel**: whether your fuel reaches the destination. The consumption figure learns from your earlier trips with the same cargo, and a reserve (the larger of 15 litres and 8% of the tank) is kept that it never plans on. It also shows what a full tank costs at your fuel price
- **Fine risk**: a warning when you have been at least 8 km/h over the limit for more than a few seconds. It is an estimate: the game does not say where the cameras are

It appears on the HUD and as a card on the Dashboard.

## The window (Delete)

| Tab | Contents |
|---|---|
| **Home** | Your driver level, what is new, your week at a glance (net income against your goal, jobs, score, net per hour), three weekly challenges, your last trip with its route and a tip |
| **Dashboard** | Truck condition, current job, the trip assistant, a two-minute speed chart, a coach summary and your latest deliveries; on a coach job the passenger rating with a chart, the timetable and a punctuality score. "Arrange this page" moves or hides sections |
| **Coach** | The score for the trip you are driving now (with technique), what to improve and what was measured |
| **Logbook** | Deliveries and coach jobs (search, sort, a full report with the route map and the speed and fuel charts, share trip card), Statistics (totals, weekly income, top cargo and routes, records, coach totals) and Compare |
| **Insights** | Reports for this week, this month and all time, charts, an income goal, where the money goes, and your best and worst job |
| **Profile** | Your level and title, 20 badges with their progress, your clean-job streak, the weekly challenges and your personal bests |
| **License** | Your key, days left, and the buttons to activate or re-check |
| **Settings** | Themes, units, HUD size, opacity, position and layout, the hints and cards, night dimming, profiles, fuel price and updates |
| **About** | Version, controls, where your files are, support and credits |

## Driving coach

Every trip is scored for **Economy**, **Safety**, **Smoothness** and **Technique**, giving an overall grade from A to F with ranked tips. It measures hard braking and launches, speeding, idling with the engine on, coasting, cruise control on fast roads, revs, driving while tired and cargo damage, and from version 0.4.0:

- **Steering**: above 54 km/h, quick left-right-left corrections within about two seconds and very fast steering movements cost points. Bends in the road do not
- **Gears and engine braking**: an engine labouring at low revs with the throttle down, braking downhill with the pedal instead of the retarder or the engine brake, and (on a manual gearbox, seen by the clutch pedal) upshifting at very high revs. An automatic gearbox is never blamed for its shifts
- **Brake heat**: over 200 degrees is hot and over 300 is very hot
- **Parking and reversing**: a normal park is one reverse and one small adjustment; every extra change of direction in the same manoeuvre is a correction
- **Rough roads**: sharp up-and-down movements at speed, and damage to the cargo within two seconds of one. They add a tip

Technique counts 15% of the overall score when there was enough driving to judge it (the overall is then 34% economy, 30% safety, 21% smoothness and 15% technique); otherwise it is 40%, 35% and 25% as before. Steering needs about two minutes at speed, gears and brakes about three minutes of driving, and parking some reversing.

The score limits are first estimates and will be tuned with real drives, so treat the numbers as guidance.

## ETS2 Coaches DLC

During a coach job (a tour or a bus line) the Dashboard shows:

- **Passenger satisfaction**: how happy the passengers are right now, with a small chart of how the rating developed during the job
- **Status chips**: the kind of job (a tour with its viewpoints, or a bus line with its stops), how punctual you have been, whether you are running late, and how many passengers are on board
- **Timetable**: one row per stage with the planned and actual times, boarding and alighting, and a chip showing how late or early you are
- **Expected income**, and the distance driven so far against the planned distance

Punctuality is scored from the actual arrival times. A stage that arrives on time, up to 5 minutes late, or early scores 100, 15 minutes late scores 80, 30 minutes late scores 50 and 80 minutes late scores 0. The score is the average over the stages you have finished. Coach hints cover being behind the timetable, hard braking and launches that the passengers feel, and a falling rating. Rest hints stay quiet during a coach job, because a bus has no rest rule.

After the job a summary card compares what it paid with what the game expected, and the distance driven with the planned one, and shows how many passengers you carried, how they rated you and how punctual you were. The job is saved in the Logbook as a Coach tour or a Bus line. Coach jobs do not count in the truck fuel average.

The coach job names come from what other developers saw the live game send, because SCS has not published them. The punctuality score and the coach hints are first estimates that will be tuned with real drives.

## Logbook

One line per delivery or coach job, stored locally in `%LOCALAPPDATA%\TcdCoDriver\logbook.tsv`.

- Search and sort deliveries; filter for scores of 80+
- Full report per delivery: score breakdown, income, fuel cost, fines, tolls, ferry, net income and net per hour
- **Route map and charts**: the route of the trip with the places where you were over the limit, braked hard, paid a fine, toll or ferry, refuelled or damaged the cargo, and charts of the speed and the fuel along the way. The routes of the newest 150 trips are kept in `%LOCALAPPDATA%\TcdCoDriver\traces`
- **Compare**: one trip against the ten before it and against your best
- **Share trip card**: saves a page of the trip in `Documents\TCD Co-Driver` and copies a short text to the clipboard. It is a file on your computer; nothing is uploaded
- Coach jobs also carry the passengers' rating, punctuality, passengers carried, the income the game expected and the planned distance
- Statistics: totals, net per hour and per distance, last 8 weeks, top cargo and routes, records, and coach totals once you have driven a coach job
- **Export CSV** saves a spreadsheet in your Documents folder and opens in Excel in any language

Your logbook, routes, scores and settings stay on your computer. They are not sent to us.

## Insights and Profile

- **Insights**: this week, this month and all time against the period before (net income, jobs, distance, net per hour, average score), an income goal for the week, charts of net income, score and fuel cost, what the money goes on, your best and worst job and what paid most
- **Profile**: experience for every job (more for a clean, punctual, well-scored one) gives you a level and a title. There are 20 badges with their progress, a streak of clean jobs in a row, three weekly challenges and your personal bests. Everything is worked out from your logbook, so nothing extra is stored, and an older logbook counts too
