# savemysunnysky.org — Website Backup

Static archive of https://www.savemysunnysky.org/ ("Save My Sunny Sky",
a community site about airplane noise around Sunnyvale / San Jose airports).

- **Archived:** 2026-10-05
- **Method:** `wget --mirror` (HTML pages) + direct download of all
  `lh7-us.googleusercontent.com` images referenced by the pages.
- **Contents:** 74 HTML pages with full text content.
  Open `www.savemysunnysky.org/index.html` in a browser to browse offline.

## Notes

- The site is built on Google Sites (new Sites), so pages are the
  JS-viewer HTML snapshots; all visible text content is preserved.
- Images are hosted on `lh7-us.googleusercontent.com` and are archived
  locally under `www.savemysunnysky.org/images/` (156 files, ~67MB) —
  Google Sites image URLs carry expiring signatures (direct curl gets 403),
  so they were re-fetched page-by-page with fresh URLs and a browser
  Referer on 2026-10-05, then rewritten to relative local paths.
  Pages now render fully offline.
- External outbound links (FAA PDFs, city documents, YouTube embeds,
  Google Drive embeds) were intentionally left as live links — they point
  to third-party documents not hosted on savemysunnysky.org.
- Google Fonts / gstatic framework files were not archived (loaded from
  CDN at view time).
