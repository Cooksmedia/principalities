# PRINCIPALITIES

A first-person spiritual warfare shooter. A special task force operative battles
Shades, Powers, and the Principality itself in the Strongholds — places where
the seen and unseen worlds meet.

*"For we wrestle not against flesh and blood, but against principalities,
against powers, against the rulers of the darkness of this world..."* — Eph 6:12

## Play

The game is a single self-contained file: **index.html** — desktop + mouse required.

- **WASD** move / **SHIFT** sprint / **MOUSE** aim / **CLICK** fire
- **R** reload / **1** Fists of Light / **2** Light Pistol
- **G** throw holy water / **HOLD RIGHT-CLICK** Shield of Faith

## Structure

- `index.html` — the playable build (all assets embedded)
- `manifest.json` — asset registry (also the schema the MCP server will serve)
- `assets/raw/` — original generated art, named `Category-name-state.png`

## Asset pipeline

Art is generated (ChatGPT/Flux) on pure black backgrounds → flood-fill cutout →
WebP compression → embedded into the build. See manifest.json for what exists
and what's still needed (`"needed"` / `"status"` fields).
