# Chandra Pratti — Portfolio

A one-page portfolio site for Chandra Pratti, Lead UX Designer. Plain HTML/CSS/JS — no build step, no dependencies to install.

## Publish it with GitHub Pages (free, ~5 minutes)

1. **Create a repository**
   Go to [github.com/new](https://github.com/new). Name it whatever you like —
   if you name it exactly `your-username.github.io`, your site's URL will be
   `https://your-username.github.io` (no repo name in the path). Any other
   name works too, it'll just live at `https://your-username.github.io/repo-name`.
   Set it to **Public**.

2. **Upload these files**
   On the repo page, click **Add file → Upload files**, drag in everything
   from this folder (`index.html`, `.nojekyll`, `README.md`, `LICENSE`),
   and commit.

3. **Turn on Pages**
   Go to **Settings → Pages** (left sidebar). Under **Build and deployment**,
   set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
   Save.

4. **Wait ~1 minute, then visit your URL**
   GitHub will show the live URL at the top of that same Pages settings
   screen once it's built. It'll look like:
   `https://your-username.github.io/` or `https://your-username.github.io/repo-name/`

That URL is permanent (as long as the repo exists and stays public) and free —
share it on your resume, LinkedIn, or with recruiters directly.

## Files in this package

| File | Purpose |
|---|---|
| `index.html` | The entire site — HTML, CSS and JS in one file |
| `.nojekyll` | Tells GitHub Pages to serve the file as-is, skipping Jekyll processing (prevents build issues with files/folders starting with `_`) |
| `LICENSE` | MIT license for the code itself (optional — delete if you don't want one) |
| `README.md` | This file |

## About the case-study images

The five case-study screenshots are currently linked directly from your old
Wix portfolio (`chandraux.wixsite.com`). That works fine right now, but if
you ever take that Wix site down, those images will break here too.

To make this site fully independent:
1. Download the 5 images you want from your Wix site (right-click → Save
   Image As).
2. Put them in a new `assets/img/` folder next to `index.html`.
3. In `index.html`, search for `static.wixstatic.com` and replace each of
   those 5 URLs with a relative path, e.g. `assets/img/verizon.jpg`.
4. Re-upload / commit the changed files.

## Updating content later

Everything is in `index.html` — no separate data file or CMS. Open it in
any text editor (or ask Claude to edit it for you) and search for the
section you want to change: hero text near the top, each case study is
inside an `<article class="sheet ...">` block, experience timeline is
under `id="experience"`, contact details are in the `<footer>` at the
bottom.

## Custom domain (optional)

If you buy a domain later (e.g. `chandrapratti.com`), add a file named
`CNAME` (no extension) to this repo containing just the domain name, then
point your domain's DNS at GitHub Pages per
[GitHub's custom domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
