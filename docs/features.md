# Features

> **Where things live:** the public overview and prices are on the [landing page](https://thecodingdad-tisonk.github.io/tcd-codriver/), accounts and keys are on the license site linked there, and these guides are in [this repo](https://github.com/TheCodingDad-TisonK/tcd-codriver-docs).

## The HUD

Drawn inside the game window while you drive. The cab has its own speedometer and turn signals, so while you are on a job the main panel shows what the cab does not: where you are going and how you are doing. Some parts are always there:

- **Status chips**: lights, parking brake, cruise control, low fuel, oil, temperature, battery and air pressure, only when switched on
- **Coach strip**: one short hint when it matters (over the limit, time to rest, long idling, high revs)
- **Trip score**: a ring with your running score and grade for the current trip
- **Summary card**: a card after each delivery with your score, net income and the top tip

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

## The window (Delete)

| Tab | Contents |
|---|---|
| **Dashboard** | Truck condition, current job, a two-minute speed chart, a coach summary and your latest deliveries; on a coach job the passenger rating with a chart, the timetable and a punctuality score |
| **Coach** | The score for the trip you are driving now, what to improve and what was measured |
| **Logbook** | Deliveries and coach jobs (search, sort, full report) and Statistics (totals, weekly income, top cargo and routes, records, coach totals) |
| **License** | Your key, days left, and the buttons to activate or re-check |
| **Settings** | Units, HUD size, opacity and position, coach hints, trip score, route line, delivery summary, the delivery and coach job HUDs and fuel price |
| **About** | Version, controls, where your files are, support and credits |

## Driving coach

Every trip is scored for **Economy**, **Safety** and **Smoothness**, giving an overall grade from A to F with ranked tips. It measures hard braking and launches, speeding, idling with the engine on, coasting, cruise control on fast roads, revs, driving while tired and cargo damage.

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
- Coach jobs also carry the passengers' rating, punctuality, passengers carried, the income the game expected and the planned distance
- Statistics: totals, net per hour and per distance, last 8 weeks, top cargo and routes, records, and coach totals once you have driven a coach job
- **Export CSV** saves a spreadsheet in your Documents folder and opens in Excel in any language

Your logbook, scores and settings stay on your computer. They are not sent to us.
