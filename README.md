# Jep4x8 Website

A static showcase for the Jep4x8 mobile horror game catalog, with a featured latest-release section for **Banshee Playtime: The Fear**. Fonts are self-hosted, game-card icons use optimized WebP assets, and both pages apply a restrictive content security policy.

## Local preview

Open `index.html` in a browser, or run a local static server from this folder:

```powershell
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## GitHub Pages

1. Push this folder to the desired GitHub repository. For the free `github.io` domain, use a user or organization site repository named `<owner>.github.io`, or configure a custom domain for the Pages site.
2. In the repository, open **Settings → Pages**.
3. Select **Deploy from a branch**, choose the publishing branch and `/ (root)`, then save.
4. Add the resulting site URL to each applicable Google Play developer listing as the website URL. AdMob looks for `app-ads.txt` at the hostname root (`https://<hostname>/app-ads.txt`). A GitHub Pages project site URL such as `https://<owner>.github.io/<repository>/` serves files under that repository path, which does not put this file at the required hostname-root URL. Use a user/organization site or a custom domain that serves this site at its root.
5. Set each game’s privacy-policy URL to `<site-origin>/privacy.html`.

GitHub Pages publishes the site publicly even when its source repository remains private. The source repository can stay private only if the organization’s GitHub plan supports Pages from private repositories; otherwise, keep it private and choose whether to upgrade the plan or make the source public before enabling Pages.

The `app-ads.txt` in this repository is copied from the seller file currently linked by the existing Play Store website entry. Keep it synchronized with the publisher’s authorized seller records. Google Play’s website field must point to the deployed site origin for ad crawlers to discover the root file.

## Privacy and security

- The site is static and does not use analytics, advertising scripts, forms, or sign-in. Local assets and a restrictive content security policy reduce third-party and injection exposure.
- Keep private contact details and credentials out of this repository. The current privacy contact is the Jep4x8 support address; replace it with a dedicated brand address if desired before launch.
- GitHub Pages may log visitor IP addresses and related request data for security. See GitHub’s [Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-privacy-statement).

## Files

- `index.html` — responsive landing page, latest-release feature, and game catalog
- `privacy.html` — account-wide privacy policy
- `app-ads.txt` — current authorized seller records
- `styles.css` — site styles and local font declarations
- `assets/` — Jep4x8 mark, generated hero and Banshee feature artwork, optimized WebP app icons, and licensed local font files
