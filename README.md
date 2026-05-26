# Neelesh Saxena — Personal Site

A one-page personal website / portfolio with sections for bio, skills, education, work experience, portfolio gallery, ideologies, and a contact form. Built in 2016–2017 while the author was a graduate student at Northeastern University.

## Live site

https://neeleshsaxena.github.io

## Tech

Static HTML/CSS/JS deployed via GitHub Pages on the `master` branch. Stack: Bootstrap 3, jQuery, [fullPage.js](https://alvarotrigo.com/fullPage/) for vertical section scrolling, WOW.js + Animate.css for scroll-triggered animations, Lightbox and Fancybox for the portfolio gallery, Font Awesome icons, Google Maps JS API for the contact-section map, and [EmailJS](https://www.emailjs.com/) for the client-side contact form. Google Analytics is wired up via `analytics.js`.

## Repo layout

- `index.html` — entire site (single-page, anchor-based navigation)
- `css/` — Bootstrap, Animate, Font Awesome, fullPage, Fancybox, Lightbox, plus `main.css` / `responsive.css` and a `presets/` folder of color themes
- `js/` — vendor libraries (jQuery, Bootstrap, fullPage, WOW, Lightbox, Fancybox, etc.) and `main.js` / `map.js` for page behavior
- `images/` — slider backgrounds, portfolio thumbnails, logos, profile photos
- `fonts/` — Font Awesome / icon font files
- `docs/` — downloadable resume PDF linked from the About Me section
- `sendemail.php` — legacy server-side mail script (the live form uses EmailJS instead)
- `*.txt` — scratch/backup snippets (`portfolio.txt`, `pagescroll.txt`, `intialSpinnerLoader.txt`, `trigger.txt`); not loaded by the site

## Editing

GitHub Pages auto-deploys from `master`, so any push to that branch updates the live site within a minute or two.

```bash
git clone https://github.com/neeleshsaxena/neeleshsaxena.github.io.git
cd neeleshsaxena.github.io
# edit index.html (and assets under css/, js/, images/ as needed)
# open index.html directly in a browser to preview locally
git add -A
git commit -m "Update site content"
git push origin master
```

The contact form is configured client-side via the EmailJS user ID embedded in `index.html`; updating the destination address means updating the EmailJS template, not this repo.

## Template credit

No upstream HTML template is explicitly attributed in the source (footer reads "Crafted By © Neelesh Saxena"). The design is a custom Bootstrap 3 one-pager that leans on the common combination of fullPage.js + WOW.js + Animate.css that was popular in mid-2010s portfolio themes; vendor libraries retain their original licenses in their respective files under `css/` and `js/`.

## Notes

- Last meaningful content update was in 2017, so the bio, role, and education sections reflect that point in time and may need a refresh.
- The site loads jQuery twice (a local copy plus the Google CDN copy) and pulls some assets over `http://`; harmless but worth cleaning up if the site is ever modernized.
