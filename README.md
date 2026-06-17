# CAIRN — Director Console

A single-file browser prototype that simulates a fictional 5v5 esport called **Cairn**. No build step, no dependencies — just open `index.html`.

**▶ Play it:** https://ajhollowayvrm.github.io/cairn-director/

## What it is

You're the director of a living competitive circuit. Press **Sim season** and the league plays itself out: matches are decided round-by-round in one permanent arena (the *Yard*) over a roaming objective (the *ember*), results feed the **GRAVL Standings**, and careers age, develop, retire, and move between teams across two divisions with promotion and relegation.

The hook: only winning a **Major** lets a team lay a permanent **cairn** on the arena floor. An elite player or team that never wins one is *unmarked* — the sport's central tragedy. The arena slowly becomes a graveyard of history.

## Playing

- **Sim season** — advance the circuit one season.
- **Skip 5 seasons** — fast-forward.
- **Reset to Season Zero** — start a fresh timeline.
- When a season's **Major** comes up, open the **Broadcast** tab to call it round-by-round, or let it auto-sim.

Explore the rest through the tabs: the story feed, live broadcast, calendar, standings, players (tap any name for a scouting card with editable attributes and commissioner controls), teams, the transfer market, the Yard of cairns, ongoing storylines, and the Annals (GOATs, Moments, Upsets, Chokes).

## A note on AI narration

The "✦ Have the desk call it" buttons are designed to call an LLM to write Major-final recaps. They only work inside an environment that proxies the Anthropic API with credentials — they will **not** work on GitHub Pages or as a plain local file, and that's intentional: a static public site can't hold an API key safely. When the call fails, the app falls back to its built-in wire copy. The simulation itself is fully functional without it.

## Tech

Plain HTML + CSS + vanilla JavaScript in one file (`index.html`). Everything — the match engine, season loop, career system, and rendering — is self-contained.
