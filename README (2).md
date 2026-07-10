# AMS Toolkit v2

Internal EdWeek Advertising & Marketing Solutions proposal-building widget. Hosted for convenience — not indexed by search engines.

## Live URL (after setup)

`https://<your-github-username>.github.io/ams-toolkit-v2/`

## First-time setup (do once)

1. **Create the repo on GitHub**
   - Go to https://github.com/new
   - Name: `ams-toolkit-v2`
   - Set visibility to **Public** (required for free GitHub Pages)
   - Do NOT initialize with a README (we already have one)
   - Click **Create repository**

2. **Upload these three files**
   - On the new empty repo page, click **uploading an existing file**
   - Drag in `index.html`, `robots.txt`, and `README.md`
   - Commit directly to `main`

3. **Enable GitHub Pages**
   - Repo → **Settings** → **Pages** (left sidebar)
   - Source: **Deploy from a branch**
   - Branch: **main** / folder: **/ (root)**
   - Click **Save**
   - Wait ~1–2 minutes. The URL appears at the top of the Pages settings page.

4. **Test the URL** in a private/incognito window to confirm it loads without needing to be signed in to GitHub.

5. **Share the URL** with the team (email or Slack). Bookmark it.

## Updating the widget later

- Edit `index.html` locally (or use GitHub's web editor)
- Commit → live in ~1 minute
- Old versions are always recoverable via GitHub's commit history

## Security posture

This site is public but takes several steps to stay out of search results and off casual radar:

- Meta tags: `noindex, nofollow, noarchive, nosnippet` (in `index.html` `<head>`)
- `robots.txt` blocks all major search engines and AI crawlers
- Referrer policy: `no-referrer` (outbound clicks don't reveal the URL)
- Repo name is generic ("ams-toolkit") — no "EdWeek" or "proposal" in the URL
- Page title is generic ("AMS Toolkit") — reduces exposure if snippet ever appears

The URL is discoverable only to people who have the link. Treat the link like an internal password: don't post it publicly, don't share with prospects, don't include in marketing materials.

## What's inside

A single-file HTML widget that:
- Collects client info, campaign timing, and product/schedule selections
- Generates a `BUILD_PROPOSAL` JSON payload
- Rep pastes payload into the "AI-Powered Sales Decks/Proposals" Claude project along with the current media kit .pptx
- Claude assembles the final proposal deck

Product catalog, rates, and slide-number hints are embedded. Update this file when the media kit or rate card changes.

## Contact

Josh Ford — jford@educationweek.org
