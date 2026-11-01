# Zebra Designs

The studio hub — showcases the apps and hosts every app's privacy policy in one place.

## Structure

```
zebra-designs/
├── index.html              # Landing page (self-contained: animated hero + app grid + privacy matrix)
├── assets/css/policy.css   # Shared stylesheet for the four policy pages
├── cubecracker/            # /cubecracker  → CubeCracker privacy policy
├── snagly/                 # /snagly       → Snagly privacy policy
├── numberbuddies/          # /numberbuddies→ Number Buddies privacy policy
├── aisle-and-grace/        # /aisle-and-grace → Aisle & Grace privacy policy
├── 404.html
├── CNAME                   # zebradesigns.app
└── .nojekyll
```

Policy URLs are path-based, e.g. `https://zebradesigns.app/snagly`.

## Deploy (GitHub Pages)

1. Create a repo (e.g. `zebra-designs`) and push this folder's contents to the default branch.
2. Repo → **Settings → Pages** → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
3. Point the `zebradesigns.app` DNS at GitHub Pages (A/ALIAS records) — the `CNAME` file is already set.

`.nojekyll` is included so GitHub serves the files as-is.

## Notes

- **Contact** is `hello@zebradesigns.app` across the hub and all four policies (this also fills the placeholder Number Buddies previously had).
- **CubeCracker's policy was newly written** — it's the only ad-supported app (Google AdMob + Firebase Analytics + Play Billing + on-device camera); the policy reflects exactly what the app declares.
- Snagly and Aisle & Grace also keep their own live sites (`snagly.house`, `aisleandgrace.com`); these copies are the studio-wide source of truth.
- Fonts (Syne / Figtree / Space Mono) load from Google Fonts; everything degrades to a system stack if they're unavailable.
