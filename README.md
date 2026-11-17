# Drydock

A single-page Star Citizen fleet, wing and CCU tracker. One file, no build step,
no server code.

## Hosting it

Upload `index.html` to a GitHub repository and turn on GitHub Pages
(Settings -> Pages -> Build and deployment -> Deploy from a branch -> `main` / `/root`).
The site appears at `https://<your-username>.github.io/<repository-name>/`.

## Where the data lives

Nothing is stored in this file. Your fleet, groups and CCU chains are saved in
your own browser, on the machine you use. They are not uploaded anywhere and
nobody visiting the site can see them — a visitor gets an empty Drydock.

Because the data is per-browser, it does not follow you between computers. Use
**Save a backup** on the Fleet tab to write a `drydock-backup.json`, and drop
that same file into **Import** on the other machine to restore it.

Clearing your browser's site data for this domain erases the fleet. Keep a
backup file if that would hurt.

## What it loads from the internet

Only the three webfonts, from Google Fonts. Everything else — the ship
catalogue, the specifications, the prices — is inside `index.html`.

## Where the ship data came from

- Pledge prices: the UEX pledge-store listing.
- Specifications and store copy: the Roberts Space Industries ship matrix.
- Lore: Star Citizen Tools.

The page footer carries the dates these were read. Prices go stale; the
Ship index lets you override any of them by hand.
