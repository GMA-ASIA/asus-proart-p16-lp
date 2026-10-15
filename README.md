# ASUS ProArt P16 · "One laptop. A whole team inside." (landing page draft)

Campaign landing-page draft for the ASUS ProArt P16 (H7607) workshop. It's a static site with no build step: `index.html` plus `assets/`.
`index-v1.html` is the first, non-Apple-style version, kept for comparison.

**Status: DRAFT, not approved by ASUS.** The repo is private and the page carries `noindex`.

## View it locally
```
git clone https://github.com/GMA-ASIA/asus-proart-p16-lp.git
cd asus-proart-p16-lp
python -m http.server 8765
```
Then open http://localhost:8765. Use a local server rather than double-clicking the file, so the video and fonts load.

## Going live on GitHub Pages (only after approval)
GitHub Pages on this account needs the repo to be **public**, and the site is visible to anyone with the link.
```
gh repo edit GMA-ASIA/asus-proart-p16-lp --visibility public --accept-visibility-change-consequences
gh api -X POST repos/GMA-ASIA/asus-proart-p16-lp/pages -f "source[branch]=main" -f "source[path]=/"
```
Link (live 1–2 minutes later): https://gma-asia.github.io/asus-proart-p16-lp/
Every push to `main` then republishes automatically.
Before going public, remove `robots.txt` and the `noindex` meta if the page should appear in search.

## Reusing this for another laptop
See the TEAMATE kit in `Desktop\asus\Website Building asset\TEAMATE`: asset checklist, content sheet, prep script and ChatGPT prompt.
