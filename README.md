# Void Lord's Blacklist Challenge

A League of Legends champion roulette. Spin the wheel, get assigned a champion revealed in their **rarest skin**, then survive the run: win to build your streak, lose and that champion is **blacklisted** from the wheel for good.

![Void Lord's Blacklist Challenge](og-image.jpg)

## Features
- **Spin-to-assign wheel** of every current champion, drawn on an HTML5 canvas with mastery rings.
- **Rarest-skin reveal** — surfaces the highest-rarity skin per champion (Mythic / Legendary / Ultimate / Exalted / Transcendent) with HD splash art and animated splashes where available.
- **Champion voice lines** on reveal — English by default, with an EN / TR toggle (remembered between visits).
- **Run mechanics** — win streaks, the Zilean revival, an ever-growing blacklist, and a full game-over summary.
- **Optional Riot account** — connect with your own dev key for mastery, match history, LP tracking, and live-game detection. Completely optional; the wheel works fully without it.
- Wins history, session log, undo, and a persistent local save.

## Play
Open the site, pick your voice language on the entrance screen, click **Enter the Rift**, then click the wheel to spin.

## Run locally
It's a single static page — no build step.
```bash
npx serve .        # or any static server
# or simply open index.html in a browser
```

## Deploy (Netlify)
Drag this folder onto <https://app.netlify.com/drop>, **or** connect this repo to Netlify for automatic deploys, **or**:
```bash
npm i -g netlify-cli && netlify deploy --prod
```
After your first deploy, set the `og:image` / `twitter:image` tags in `index.html` to your absolute URL for the best link previews.

## Tech
Vanilla HTML / CSS / JavaScript, HTML5 canvas, the Web Audio API, and the public **Data Dragon** and **Community Dragon** APIs. No frameworks, no build.

## Credits & legal
League of Legends and all related champion art, names, and voice lines are property of **Riot Games, Inc.** This is an **unofficial fan project** and is **not affiliated with or endorsed by Riot Games**. Game data and assets are served from Riot's public Data Dragon and the community-run Community Dragon project.

## License
The project's own source code is released under the MIT License (see [`LICENSE`](LICENSE)). This applies to the code only — not to Riot Games' assets.
