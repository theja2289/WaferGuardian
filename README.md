# Wafer Guardian

A small browser game about wafer test and probe cards. Match the probe card to the chip, load the wafer, run the prober and catch the bad dies. Then build a MEMS probe card yourself: design the spring, grow it with lithography, let the robots assemble it, and measure every tip.

Two reference pages sit alongside the game: **The industry** (who makes probe cards, where, with what technology and revenue, on a world map) and **The robotics case** (interactive models of why flexible automation beats dedicated cells as design cadence rises). Company figures come from 2025 filings and are marked where estimated; the robotics models are illustrative.

Play it: https://theja2289.github.io/WaferGuardian/

## Run locally

Open `index.html` in a browser. No build step, no dependencies.

## Add a chip or a probe card

Two ways:

- **In the game.** Open Workshop from the home screen. Every chip and probe card is editable there, you can add your own, and the changes are saved in your browser. Export and import the whole set as JSON to share it.
- **In the file.** Edit the `DEFAULT_CHIPS` and `DEFAULT_CARDS` tables at the top of the script in `index.html` to change what everyone gets. The match rules (pad pitch, pad layout, current, dies per touchdown, full-wafer contact) and the spec cards all read from those tables.

## Note

Specs are simplified for play. Probe card manufacturing is described at the level of public MEMS probe card literature.
