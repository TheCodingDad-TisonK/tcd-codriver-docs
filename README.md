# TCD Co-Driver: documentation

TCD Co-Driver is a co-driver plugin for **Euro Truck Simulator 2** and **American Truck Simulator** on Windows. It draws a heads-up display inside the game and keeps a driving coach and a logbook of every delivery.

Official website: https://thecodingdad-tisonk.github.io/tcd-codriver/

This repository contains **documentation only**: guides, changelog and the legal pages. It does not contain the plugin source, the license server, keys, or any account data. The plugin and its license service are distributed through the website above.

## How the three pieces fit together

| Piece | Address | Purpose |
|---|---|---|
| **Landing page** | https://thecodingdad-tisonk.github.io/tcd-codriver/ | The public front door: what the plugin is, features, price and legal pages. Static and always online. |
| **License site** | https://unhistorical-subglobular-marhta.ngrok-free.dev | The running server: accounts, keys, email, license checks and payments. |
| **These docs** | https://github.com/TheCodingDad-TisonK/tcd-codriver-docs | Guides, FAQ and changelog. No source code and no secrets. |

People start at the landing page and click through to the license site to get a key. The plugin checks licenses with that server, and these docs explain how to use everything.

## Start here

- [Installation](docs/installation.md): install the plugin and activate your key
- [Features](docs/features.md): what the HUD, dashboard, coach, Coaches DLC support and logbook show
- [Licensing and payments](docs/licensing.md): trial, subscription, PayPal and offline use
- [FAQ](docs/faq.md): common questions and problems
- [Changelog](docs/changelog.md): what changed in 0.3.0
- [Legal](legal/): terms of service, privacy policy and legal notice

## Support

Use the contact form on the website. If something does not work, include the end of the game log:

```
Documents\hry_core\ets2\hry_core.log
```

(or `...\ats\hry_core.log` for American Truck Simulator).

TCD Co-Driver is an independent product. It is not made, endorsed or supported by SCS Software. Euro Truck Simulator 2 and American Truck Simulator are trademarks of SCS Software.
