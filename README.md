# Mayo Entrepreneurship Club

Club website: https://quantumshawn.github.io/entrepreneurship-club/

One page (`index.html`) plus photos in `images/`. It uses the same design system as mayoasa.com (Big Shoulders Display, Inter, IBM Plex Mono, paper background, kicker labels, pill buttons, striped cards), with Mayo's forest green and Vegas gold as the accents. Edit, commit, push, and GitHub Pages updates the live site in about a minute.

## Swap in real photos

The photos in `images/` are free Unsplash placeholders. Replace a file with your own photo **using the same file name** and it shows up in the same spot. Keep each under ~400 KB so the page loads fast on phones.

| File | Where it shows | Best shape |
| --- | --- | --- |
| `hero.jpg` | Full-screen photo at the top (gets a dark green overlay so the text stays readable) | Wide landscape, 1600+ px |
| `why.jpg` | Next to "This is where you start" | 4:3 landscape |
| `first-meeting.jpg` | Next to "Leave with a team and an idea" | 4:3 landscape |

After swapping, update each photo's `alt="..."` text in `index.html` to describe the new photo. Once they're all your own, delete "Photos from Unsplash" in the footer.

## Founder photos

Founders show initials circles for now. To use a real photo (like on mayoasa.com), add e.g. `images/founder-gates.jpg` and replace that card's `<span class="avatar-slot" ...>G</span>` with:

```html
<div class="avatar-slot" style="padding:0;overflow:hidden"><img src="images/founder-gates.jpg" alt="Gates" style="width:100%;height:100%;object-fit:cover"></div>
```

## Competitions and the countdown

Each competition in the season timeline is an `<li class="event">` with a `data-deadline` (date, time, and time zone offset). The page uses those to:
- show a live countdown to the next deadline (in the season section and the stat bar)
- move the "Today" marker
- grey out and tag past competitions as "Closed" automatically

To add or change one, copy an existing `<li class="event">` block and edit the deadline, name, tags, prize, and description. Keep them in date order.

## Other edits

- **Add Instagram:** search `index.html` for `INSTAGRAM` in the footer.
- **Change meeting time or room:** search for `3:45` and `Priebe` (hero, CTA band, footer, page description).
- **Contact email:** assembled in the script at the bottom (`1005588` + `rochesterschools.org`) so spam bots scraping the page don't pick it up. Change it there.
