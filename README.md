# MediaKit website

English, responsive static pages built with HTML and one shared CSS file. No JavaScript, framework, package installation, build step, or remote font dependency.

## Pages

- `index.html`: product introduction, features, app previews, and release availability.
- `support.html`: native HTML FAQ disclosures and contact links to `support@mediaprocess.com`.
- `assets/styles.css`: shared tokens, desktop/mobile layouts, focus styles, and print rules.
- `assets/images/`: existing App artwork and English screenshots copied from the parent workspace.

Navigation and footer markup are intentionally duplicated across the two pages. Keep them in sync when adding a page.

## Local preview

From this directory:

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

Open `http://127.0.0.1:4173/`. You can also open the HTML files directly. All local page and asset links are relative, including links to FAQ sections, so the site can be hosted under a project path.

## Content and launch

The download area currently states “Coming soon to the App Store.” Replace it with the verified App Store URL when available. Do not use development StoreKit prices as public offers.

The current screenshots are existing development app captures, used intact and labeled as previews. Re-capture them against the release build before launch. The brand is MediaKit; the underlying app project is still named Media Process.

Privacy and Terms pages are a subsequent phase. Their links are intentionally omitted until real pages and approved content exist. No invented policies, legal operator, or dead download links are included. Confirm the operating entity and final domain before adding copyright attribution, canonical URLs, sitemap, and social-image URLs.

The Git remote currently belongs to `MediaProcess/mediakit.github.io`. The repository name alone does not establish `https://mediakit.github.io`; confirm the actual Pages URL before release. `.nojekyll` allows serving the static files directly. No deployment has been performed as part of this implementation.

## Manual checks

Check both pages at 375px, 768px, and 1440px, plus a narrow 320px view. Follow the feature, support, availability, topic, and back-to-top links. Tab through navigation and open/close FAQs with Enter or Space. Verify the contact address without sending an email. Check 200% browser zoom, image loading, and browser console output. Check a nested project path as well as the site root before publishing.
