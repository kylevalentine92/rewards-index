# SA Rewards Complication Index

How hard is it to get the value South African rewards programmes promise? This site scores 30 programmes out of 100 on effort, across eight dimensions and four income personas.

## What's in this repo

- `index.html`: the whole site in one file. The data is built in, and charts use d3 loaded from cdnjs.

## Publish on GitHub Pages

1. Create a new public repository on GitHub, for example `rewards-index`.
2. Upload `index.html` and this `README.md` to the root of the repository (Add file, then Upload files, then Commit).
3. Open the repository's Settings, then Pages.
4. Under Build and deployment, set Source to "Deploy from a branch", choose the `main` branch and the `/ (root)` folder, then Save.
5. After a minute or two the site is live at `https://<your-username>.github.io/rewards-index/`.

To use your own domain, add it under Settings, then Pages, then Custom domain, and follow GitHub's DNS instructions.

## Updating the data

The scores, ratings, evidence notes, personas and change log are stored as JSON inside `index.html`, in the script tag with `id="rc-data"`. Replace the file with a new build to publish an update. Visitors can download the current data with the button at the bottom of the page.

## Method in brief

Each programme is rated 1 to 5 on earning complexity, tier clarity, habit burden, redemption friction, expiry and breakage, visibility, prerequisites and fees, and rule volatility. Each rating becomes (rating minus 1) divided by 4, times its weight, and the eight are added up. Habit burden is the only part that changes by persona.

Ratings come from public programme rules and South African press coverage researched in October 2026. Persona habits are early assumptions, not measured data.

Independent. Not affiliated with or endorsed by any programme. Not financial advice.
