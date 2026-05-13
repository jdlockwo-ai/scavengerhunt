# Vindictus Scavenger Hunt GitHub Pages Package

Upload these files to a GitHub repository and enable GitHub Pages.

## Files

- `index.html` — landing page with links to the challenge list and live tracker
- `clues.html` — player-facing clue/challenge page with collapsible difficulty sections
- `tracker.html` — live scoreboard/progress tracker page

## Important Setup Step

Before publishing, open `tracker.html` and replace:

```js
const DATA_URL = 'https://script.google.com/macros/s/AKfycbzyl_u5jbO8yn1ZmZJUf1P2w62lbdncjNeSarK7KdUdJEbmLbhCGhiEyiQ62GMTfe8Y/exec?action=data';
```

with your deployed Google Apps Script web app URL, for example:

```js
const DATA_URL = 'https://script.google.com/macros/s/YOUR_DEPLOYMENT_ID/exec?action=data';
```

## GitHub Pages

1. Create a public GitHub repository.
2. Upload these files to the root of the repository.
3. Go to Settings → Pages.
4. Set Source to Deploy from a branch.
5. Select `main` and `/root`.
6. Save.

Your site will load at a URL like:

`https://yourusername.github.io/repository-name/`


Tracker URL configured for the provided Apps Script deployment.
