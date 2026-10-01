# Color game

Find the odd-colored tile before time runs out. Vanilla HTML/CSS/JS, no build step.

Cloudflare Pages hosts `color-game-web.pages.dev`; the personal site's Worker proxies it at `https://sambarbeau.com/color/`. Keep assets relative. The GitHub repository is `SamBarbeau/color-game-web`.

The board fits the available viewport after accounting for the header, stats, and result controls. Short landscape screens use a two-column layout. Rounds lock immediately on a correct answer, stop the timer during the brief transition, and reject late clicks. High-score storage is optional, so blocked localStorage does not break gameplay.

Preview with `python3 -m http.server 8002` or the sibling personal site's `scripts/preview.mjs`. Deploy through the existing main-branch integration.
