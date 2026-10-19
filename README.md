# GZX Gaming — Spin & Win

Prize wheel for the GZX Gaming lounge. Players earn a spin after an hour of play and win gaming time, drinks or snacks. A PIN-protected admin panel lets staff control every prize, slice, chance, color and text.

The whole app is one static page — no build step, no server.

```
public/
  index.html            # the spinner + admin panel
  assets/gzx-poster.jpg # background poster
netlify.toml            # Netlify publish settings
```

## Run locally

Open `public/index.html` through any static server, for example:

```bash
npx serve public
```

## Deploy (Netlify)

`netlify.toml` already points Netlify at the `public` folder. Connect this repo in Netlify, or drag the `public` folder onto Netlify Drop.

## Admin panel

- Open it with the gear icon (top-right) or **Ctrl + Shift + A**.
- Default staff PIN: `1234` — **change it under Settings → Staff PIN on every screen you use.**
- Prizes, odds, slices, colors, text, settings and spin history are saved in that browser only (localStorage). Use **Settings → Download / Load backup** to copy a setup to another screen.

The PIN keeps players out on the lounge screen; it is not real security.
