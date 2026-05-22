# NI-JAP — Anime Convention Niamey 2026

A presentation website for a Japanese pop culture event in Niamey. This project includes a vibrant landing page, neon cyber-style visuals, a live countdown, daily anime quotes, a newsletter form, and a mobile-friendly navigation menu.

## Project structure

- `index.html` — main page containing the page layout, content, and inline JavaScript logic.
- `style.css` — global styling, responsive layout, color variables, and neon Japanese-inspired visuals.
- `script.js` — currently empty; the active JavaScript is embedded in `index.html`.
- `README.md` — English project documentation.

## Features

- live countdown to the event date
- embedded Google Maps for the event location
- daily anime quote with previous/next navigation
- newsletter signup with email validation
- responsive mobile menu and smooth scrolling

## Japanese culture focus

This site is designed around the energy of Japanese pop culture:

- anime and manga references throughout the quotes section
- neon color palette inspired by Tokyo nights and modern Japanese city design
- Japanese-style typography and layout cues using Orbitron and Rajdhani fonts
- event branding centered on the otaku community and convention spirit

## Customize the event

### Change the event date

- In `index.html`, update the `EVENT_DATE` value in the embedded script.
- Also update the displayed date text in `document.getElementById('eventDateDisplay').textContent`.
- Example:
  ```js
  const EVENT_DATE = new Date('2026-05-30T15:00:00');
  ```

### Change the location

- Edit the address text in the `#section-map` section of `index.html`.
- Update the `map-detail-value` and `map-detail-sub` content.
- Replace the Google Maps `iframe` source if your venue changes.

### Change the quotes

- Modify the `QUOTES` array in `index.html`.
- Each quote object should include `q` (quote), `a` (author), and `s` (series).
- The quotes reflect Japanese anime and manga characters to keep the theme authentic.

### Change the style

- Colors are defined in `style.css` under `:root` variables.
- Adjust `--cyan`, `--violet`, `--magenta`, and other theme values to customize the look.

## Technical notes

- JavaScript is currently embedded inline in `index.html`.
- For better separation, you can move the `<script>` block into `script.js` and include it with a `<script src="script.js"></script>` tag.
- The newsletter form uses Formspree as a simple demo backend.

## Possible improvements

- move the JavaScript logic into `script.js` for cleaner HTML
- add a real email backend or a dedicated newsletter service
- improve mobile responsiveness for small screens
- add better accessibility with proper `<form>` fields, labels, and ARIA attributes

## Run the site

Open `index.html` in a browser.

For development, use a local static server or host it on a static website platform.

