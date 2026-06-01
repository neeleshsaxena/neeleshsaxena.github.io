# Neelesh Saxena — Personal Site

A single-page personal site / portfolio. Sections: bio, skills, work experience, projects, contact.

## Live site

https://neeleshsaxena.github.io

## Tech

Plain static HTML deployed via GitHub Pages from the `master` branch. Styling is Tailwind via Play CDN with a small custom `<style>` block for the retro / amber-CRT touches (typewriter intro, blinking terminal cursor, film grain). Type is JetBrains Mono for headers and Inter for body, both from Google Fonts. No build step.

## Repo layout

- `index.html` — the entire site
- `images/favicon.ico` — favicon
- `README.md` — this file

## Editing

GitHub Pages auto-deploys from `master`, so any push updates the live site within a minute or two.

```bash
git clone https://github.com/neeleshsaxena/neeleshsaxena.github.io.git
cd neeleshsaxena.github.io
# edit index.html
# open index.html directly in a browser to preview locally
git add -A
git commit -m "Update site"
git push origin master
```

## Notes

- The previous version (Bootstrap 3 + jQuery + fullPage.js + WOW.js + Lightbox + Fancybox + EmailJS contact form + Google Maps embed) was retired in 2026 in favor of this leaner build.
- Project content reflects the resume and GitHub at the time of the last edit.
