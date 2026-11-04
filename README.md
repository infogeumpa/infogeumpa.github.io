# Info Geumpa – website (GitHub Pages)

Static site for the TikTok developer app review (Login Kit + Content Posting API).

## Files
- `index.html` – home page (the one you already have, unchanged apart from the email)
- `about.html`, `tiktok.html`, `contact.html`, `privacy.html`, `terms.html`
- `404.html`, `robots.txt`, `.nojekyll`, `assets/style.css`

## Before uploading
1. Put your `index.html` in the root next to the other pages.
2. Replace the email everywhere (one command):
   `grep -rl infogeumpa@gmail.com . | xargs sed -i 's/infogeumpa@gmail.com/emailkamu@domain.com/g'`
3. In `index.html` the privacy/terms/TikTok links are relative, so they work on `user.github.io/repo/` and on a custom domain.

## Publish
Repo name must be exactly `infogeumpa.github.io` (under the GitHub account/org `infogeumpa`).
Repo -> Settings -> Pages -> Deploy from a branch -> `main` / root.
Site URL: https://infogeumpa.github.io/

## TikTok developer portal
- Website URL: `https://infogeumpa.github.io/`
- Privacy Policy URL: `https://infogeumpa.github.io/privacy.html`
- Terms of Service URL: `https://infogeumpa.github.io/terms.html`
- URL verification: download the `tiktokXXXX.txt` file TikTok gives you, put it in the repo root, push, then click Verify.
- Scopes: `user.info.basic`, `video.publish` (and `video.upload` if you want drafts).
- Note: until the app passes the audit, posts from an unaudited client are limited to private visibility.
- Prepare a demo video (screen recording): connect with TikTok login -> review video/caption/privacy -> approve -> post.
