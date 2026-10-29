# Ground Truth: Tasmania

An edu-tainment game about the residential foundation assessments engineering geologists do every day, played on a Command & Conquer-style map of Tasmania.

Pick up contracts around the state, hire a crew (or lone-wolf it), drive to site, avoid the services, drive push tubes, run DCP tests, log the soil, run the lab tests and write an AS 2870 site classification report before the deadline.

## Play

It's a single static page with no build step and no dependencies to install.

- **Locally:** open `index.html` in a browser.
- **GitHub Pages:** in the repository go to *Settings → Pages*, set the source to *Deploy from a branch*, choose `main` and `/ (root)`. The game is then served at `https://casa-vino.github.io/Ground-Truth-Tasmania/`.

Progress is saved in the browser's local storage.

## What it teaches

| Stage | In the game |
| --- | --- |
| Desk study & services | Before You Dig Australia (BYDA) plans that take two days and are only indicative, private services that never show on BYDA, surface clues, cable locators, potholing |
| Push tubes | A timing minigame with a Christie post driver: refusal, floaters and offsetting to re-drive |
| DCP (AS 1289.6.3.2) | Blows per 100 mm, when to call refusal, stuck rods |
| Field logging | Ribbon test for field texture, Munsell colour matching |
| Lab | Oven drying (12 h), crushing, plastic limit thread rolling, liquid limit by Casagrande cup (AS 1289.3.1.1) or cone penetrometer (AS 1289.3.9.1), chosen per sample, linear shrinkage (AS 1289.3.4.1), moisture content |
| Report | Casagrande plasticity chart and USCS, y<sub>s</sub> calculation, AS 2870 site class and footing recommendation |

The **Field manual** tab in the game explains each procedure.

## Game simplifications

These are deliberate simplifications. Check them against your own practice before relying on the numbers:

- I<sub>ss</sub> is estimated as 0.3 × linear shrinkage (on real jobs, run shrink-swell tests to AS 1289.7.1.1).
- A single H<sub>s</sub> of 2.3 m is used statewide, with Δu = 1.2 pF at the surface, falling to 0 at H<sub>s</sub>.
- Ribbon-length cut-offs and refusal criteria (about 20 blows/100 mm) are typical values, not a standard.
- Soil profiles for each geology are generalised and randomised.

## Options

- **Fog of war:** off by default. Switch it on from the opening screen or the map. Only areas you've driven through are revealed, and contracts in unscouted areas come without desk study notes.
