# This Day in History

An almanac-styled static page showing real historical events, births, and deaths for any date,
pulled live from Wikipedia's public "On this day" REST API.

- No backend, no build step, no API key.
- Plain HTML, CSS, and vanilla JavaScript.

## Files

```
index.html    the almanac (date picker, category tabs, one fact per "leaf")
detail.html   expanded view of a single fact
styles.css    shared design system
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Deploy

Push the folder to any static host — GitHub Pages, Netlify, Cloudflare Pages — no configuration needed.

## Data

- `https://en.wikipedia.org/api/rest_v1/feed/onthisday/{events|births|deaths}/{MM}/{DD}`
- `https://en.wikipedia.org/api/rest_v1/page/summary/{title}`

Content from Wikipedia, licensed CC BY-SA.

## License

MIT — see `LICENSE`.
