# Phone Paddle Pickleball

A browser game where your phone is the paddle. You stand on a 3D court; the screen shows the face of a pickleball paddle that is see-through while the phone is upright and turns solid as you lower it. Swing the phone to hit the ball. No build step, no dependencies: everything is in `index.html`.

## Controls
- **Phone (HTTPS link):** hold upright to watch, lower and swing when the ball glows yellow. iPhone asks for Motion & Orientation access when you tap Start.
- **Computer:** move the mouse down to lower the paddle; click or press Space to swing.
- Swing early = cross-court, late = down the line. Harder swing = deeper (too hard goes long).
- Rally scoring to 11, win by 2. Serve and return must bounce.

## Files
- `index.html` – the whole game (canvas renderer, physics, AI, motion input)
- `manifest.webmanifest`, `icon.svg` – "Add to Home Screen" support (fullscreen, portrait)
- `netlify.toml` – publishes the folder and allows motion sensors

## Deploy
1. Push this folder to a GitHub repo.
2. In Netlify: Add new site → Import an existing project → GitHub → pick the repo. Leave the build command empty and the publish directory as `.`.
3. Every push to `main` redeploys. Open the Netlify URL on your phone.

Quick alternative: drag this folder onto https://app.netlify.com/drop.
