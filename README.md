# UpCycled Woodcrafts Website

This repository contains the source for the UpCycled Woodcrafts by Margreet website.

## Project Overview

This is a static multi-page website built with:
- HTML
- CSS

Main pages:
- index.html: Home page
- gallery.html: Gallery of projects
- getaquote.html: Quote request form
- aboutme.html: About page
- contact.html: Contact page

Other important files:
- styles.css: Shared styles across pages
- CNAME: Custom domain mapping for GitHub Pages
- getaquote.html: Quote form currently submits via FormSubmit

## Repository Structure

- aboutme.html
- contact.html
- gallery.html
- getaquote.html
- index.html
- shop.html
- styles.css
- CNAME
- images/

## How Publishing Works

This site is set up to be published from GitHub using the main branch and a custom domain.

Expected production URL:
- https://upcycledwoodcrafts.com

### One-time setup in GitHub

1. Open the repository on GitHub.
2. Go to Settings > Pages.
3. Under Build and deployment, set:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /(root)
4. Save.
5. In the Custom domain field, set:
   - upcycledwoodcrafts.com
6. Keep Enforce HTTPS enabled once certificate is active.

The CNAME file in this repo should contain:
- upcycledwoodcrafts.com

## Publish New Changes

1. Make your edits locally.
2. Commit and push to main.
3. GitHub Pages redeploys automatically after each push.
4. Wait about 1-5 minutes, then refresh the live site.

## See Live Edits Before Publishing

You have two practical options:

### Option 1: VS Code Live Server (fastest feedback)

1. Install the VS Code extension Live Server (by Ritwick Dey).
2. Open index.html in VS Code.
3. Right-click the file and choose Open with Live Server.
4. A local URL opens (usually http://127.0.0.1:5500).
5. Save files to see updates automatically in the browser.

### Option 2: Local server from terminal

From the repo folder, run:

Python server:

```powershell
py -m http.server 8000
```

Then open:
- http://localhost:8000/index.html

Tip: Use Ctrl+F5 for a hard refresh if styles appear cached.

### Option 3: Open file directly

After making changes, save the file and open from file explorer in browser.

## Important Notes

- Because the quote form currently submits to FormSubmit, form submissions can still work on GitHub Pages.

## Troubleshooting

- Site did not update after push:
  - Check GitHub Actions/Pages deployment status in the repository.
  - Verify files were pushed to main.
- Domain not resolving:
  - Confirm DNS records and CNAME match upcycledwoodcrafts.com.
- Styling looks old:
  - Hard refresh (Ctrl+F5) to clear browser cache.
