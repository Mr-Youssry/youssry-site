# youssry.info

Personal site of Ahmed Youssry — Fractional CFO & Strategy Consultant. Live at <https://youssry.info>.

Plain static HTML: one page, no framework, no build step.

```
index.html             the page (styles and script inline)
img/                   images, named <name>-<hash>.webp — served with a one-year cache,
                       so a changed image needs a new filename
og-knight.jpg          1200×630 share preview (LinkedIn, WhatsApp, X…)
favicon.ico, apple-touch-icon.png
robots.txt, sitemap.xml
```

## Deploy

The site is served by Caddy from `/opt/sites/youssry` on the server. Deploying is copying the changed files:

```bash
scp index.html <server>:/opt/sites/youssry/
```

No reload is needed for content changes.
