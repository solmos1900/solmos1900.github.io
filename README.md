# solmos1900.github.io

Sebastian Olmos's personal site. Live at **[solmos1900.github.io](https://solmos1900.github.io)**.

Plain static HTML/CSS, no build step, no dependencies. Push to `main` and GitHub Pages
publishes automatically, usually within a minute.

## Structure

```
index.html               the whole site: About, Off the clock, Projects, Contact
assets/css/style.css     all styling, light/dark theme via CSS variables
assets/js/main.js        theme toggle + small interactions
pillars/privacy/         Pillars app privacy policy
pillars/terms/           Pillars app terms of use
```

## Editing

Open `index.html` and edit the text directly. Sections are marked by id
(`#about`, `#offline`, `#projects`, `#contact`) if you want to jump to one.
Styling lives entirely in `assets/css/style.css`.

## Preview locally

```
python3 -m http.server 8000
```

then open `http://localhost:8000`.

## Deploy

Commit and push to `main`. No CI, no build, GitHub Pages serves the files as-is.

## A note on `pillars/`

`pillars/privacy/` and `pillars/terms/` are linked directly from the Pillars iOS app's
App Store listing (`PillarsAppConfig.swift`). Don't rename or move these paths without
updating that file and resubmitting the app.
