# Edgar Wright's 1000+ Favourite Films — Watch Tracker

<a href="https://buymeacoffee.com/fnordcorps" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="50"></a>

A self-contained, single-file watch tracker for Edgar Wright's curated list of favourite films from a century of cinema. Tap to mark watched, ticks save in your browser, decades-grouped, searchable, no accounts, no tracking, no build step.

## What's in the list

The list was originally compiled by Edgar Wright and Sam DiSalle for [MUBI in 2016](https://mubi.com/lists/edgar-wrights-favorite-movies), then updated periodically — most recently February 2024. This tracker uses the **comprehensive "all updates" version**: every film Edgar's added across the 2016, 2017, 2022, and 2024 versions of the list, sorted by year.

**1213 films, 1920–2023.**

If you'd rather have only the strict current 1000 (with films Edgar removed in later updates pruned out), open an issue and I'll add it as a toggle.

## Features

- **One file, no dependencies** — open `index.html` in any modern browser, that's it.
- **Persistent ticks** — saved to `localStorage`, survives browser restarts.
- **Search** by title or director.
- **Filter** by All / To Watch / Watched.
- **Decade jump nav** — skip straight to the 60s, 90s, etc.
- **Live progress** — counter, percentage, progress bar.
- **Mobile-friendly** — single-column responsive layout.
- **Export / Import backup** — download your watched list as a JSON file, restore it later or on another device.
- **Reset button** if you want to start over.

## Use it

**Easiest:** [open the live version on GitHub Pages](https://YOUR-USERNAME.github.io/REPO-NAME/) *(update this link once Pages is enabled)*

**Or run it locally:**
1. Download `index.html`
2. Double-click it, or open it from your browser
3. Done. Tick stuff.

Your watched-status is stored in `localStorage` under the key `edgar_wright_1000_watched`, scoped to whichever domain you're on. That means progress saved on the GitHub Pages version isn't shared with the locally-opened version, and vice versa — same browser, different "places" as far as the browser is concerned.

### Moving progress between devices

Use the **Export backup** / **Import backup** buttons at the bottom of the page. Export gives you a small JSON file with everything you've ticked; import on another device merges those into the existing ticks (won't remove any). Backups are matched by title + year so they stay valid even if the film list is later updated.

## Hosting it on GitHub Pages

1. Push this repo to GitHub
2. Settings → Pages → Source: `main` branch, root folder
3. Wait a minute, you've got a live tracker

## Tech notes

- Vanilla HTML/CSS/JS, no framework, no build, no bundler
- Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces) (display) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (body) via Google Fonts
- ~65KB, including all 1213 film entries
- Storage uses a simple integer-id Set serialised to JSON — about 4KB max even with everything ticked

## Credits

- **The list:** Edgar Wright & Sam DiSalle. Originally on MUBI, mirrored on [Letterboxd](https://letterboxd.com/crew/list/edgar-wrights-1000-favorite-movies/) where Edgar updates it.
- **Source data:** Compiled from the 2016 list and the 2024 update.
- This project is a fan-made tracking tool. The list itself is Edgar Wright's curation — go follow him on [Letterboxd](https://letterboxd.com/crew/) for the canonical version.
- Created for the Lazy by @Fnordcorps

## License

MIT — do what you want with the tracker code. The film list itself belongs to its author.
