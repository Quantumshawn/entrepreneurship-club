# Mayo High Entrepreneurship Club

Club website: https://quantumshawn.github.io/entrepreneurship-club/

The site is one file, `index.html`, plus photos in `images/`. Edit, commit, push, and GitHub Pages updates the live site in about a minute.

## Swap in real photos

The photos in `images/` are free Unsplash placeholders. Replace a file with your own photo **using the same file name** and it shows up in the same spot. Landscape photos around 1200–1400 px wide work best; keep each under ~400 KB so the page loads fast on phones.

| File | Where it shows |
| --- | --- |
| `hero-1.jpg` | Big photo at the top |
| `hero-2.jpg` | Bottom-right photo at the top |
| `hero-3.jpg` | Small square photo at the top |
| `do-brainstorm.jpg` | Tall photo in "What we do on Thursdays" |
| `do-research.jpg` | Top-right photo in "What we do on Thursdays" |
| `do-build.jpg` | Bottom-right photo in "What we do on Thursdays" |

After swapping, update each photo's `alt="..."` text in `index.html` to describe the new photo. Once they're all your own, you can delete the "Photos from Unsplash" line in the footer.

## Competitions and the countdown

Each competition in the season timeline is an `<li class="event">` with a `data-deadline` (date, time, and time zone offset). The page uses those to:
- show a live countdown to the next deadline
- move the "Today" marker
- grey out and tag past competitions as "Closed" automatically

To add or change one, copy an existing `<li class="event">` block and edit the deadline, name, prize, and description. Keep them in date order.

## Other edits

- **Add Instagram:** search `index.html` for `INSTAGRAM` in the footer.
- **Change meeting time or room:** search for `3:45` and `Priebe` (hero, footer, and the page description near the top).
- **Contact email:** it's assembled in the script at the bottom (`1005588` + `rochesterschools.org`) so spam bots scraping the page don't pick it up. Change it there.
