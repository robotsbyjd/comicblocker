# Comic Blocker

Comic Blocker is a free, single-page storyboard and script-layout tool for comics writers.

Open `index.html` in a browser, or deploy the folder to any static host. The app stores work locally in the browser for recovery, and the main project save is a downloaded `.json` file.

## What It Does

- Block comic pages with panels and templates.
- Write page direction and panel-by-panel script entries.
- Add speech bubbles, thought bubbles, captions, SFX, and reference images.
- Use thumbnail mode to see pacing across the whole project.
- Export a PDF or compile a clean text script.
- Load the built-in tutorial from **New / Tutorial**.

## Deploy

### Vercel

1. Put `index.html`, `favicon.svg`, the logo SVG files, `preferredlogo.png`, and this `README.md` in a GitHub repo.
2. Import the repo in Vercel.
3. Use the default static site settings.
4. Add a custom domain when ready.

### GitHub Pages

1. Push this folder to a GitHub repo.
2. In repo settings, enable Pages from the main branch.
3. GitHub Pages will serve `index.html`.

## Privacy

Comic Blocker does not upload projects anywhere. Save files, autosave recovery, and imported images stay in the user's browser/computer unless the user chooses to share an exported file.

## Optional Product Analytics

Comic Blocker can send privacy-safe product events to PostHog. It is off by default.

To enable it, create a free PostHog project, copy the project API key, and paste it into the `comicblocker-posthog-key` meta tag in `index.html`:

```html
<meta name="comicblocker-posthog-key" content="phc_your_project_key_here" />
```

The app tracks interaction signals only: session duration milestones, total click count in the session summary, Ko-fi clicks, script exports, project saves, and PDF export started/completed/failed. It does not send comic text, page direction, panel scripts, imported images, project titles, or author names.
