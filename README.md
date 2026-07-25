# scalesites-au-social-assets

Public, unauthenticated image host for the Scalesites AU organic social pipeline (FB + IG),
consumed by the "Social content engine — FB+IG, all brands" routine via
`raw.githubusercontent.com/Craig-83/scalesites-au-social-assets/main/<filename>`.

Facebook fetches the image URL server-side, so this repo must stay **public** and filenames
must have **no query string**.

## How to add a creative

Push each PNG named **exactly** as the Notion Content Queue row's `Local Image Path`, e.g.
`Post-03-FAQ-Forest.png`. The next routine run's WIRE step fetches
`https://raw.githubusercontent.com/Craig-83/scalesites-au-social-assets/main/<filename>`; if it
returns HTTP 200 with an image content-type, it sets that row's `Image URL` and flips
`Status` to `Ready`.

5-colour rotation: Terracotta / Ochre / Forest / Slate-Blue / Deep-Slate.

See `reports/social/scalesites-au/README.md` in the Scale-Ops repo for the batch record.
