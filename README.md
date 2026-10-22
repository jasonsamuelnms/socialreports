# NMS Social Reports

A lightweight browser-based analytics dashboard for National Model School social content.

## Features
- Import Excel (.xlsx/.xls) and CSV reports
- Campus names, platform labels (Instagram, Facebook, Facebook & Instagram, YouTube), and manually entered post/reel titles
- Dashboard filters, charts, post table/cards, search and sorting
- Manually enter Hook Rate and Hold Rate
- Review imported rows before applying changes
- Deduplicate by post URL when available; otherwise match campus + platform + title
- Cumulative metrics (views, likes, shares, saves, comments, reach and follows) cannot decrease on update; lower incoming values are flagged and the saved higher values are retained
- Export Excel with columns: S.no Date, Reel title, Views, Likes, Share, Saves, Comments, Reach, Follows, Hook Rate, Hold Rate

## Publish with GitHub Pages
1. Open **Settings → Pages** in this repository.
2. Under Build and deployment, select **Deploy from a branch**.
3. Select branch `main` and folder `/ (root)`, then Save.
4. Wait for GitHub Pages to publish the site; the published URL appears on the Pages settings screen.

## Storage limitation
The current version stores records in the current browser's local storage. It does not yet sync across different browsers/devices or write to Google Sheets. Export Excel regularly as a backup. A shared database/API is required for true shared storage and multi-user updates.

## Import notes
Keep column headers in the first row. To match records reliably across daily uploads, include a stable post URL/link and keep the same title, campus and platform when a URL is unavailable. A newly imported file is not saved until you confirm the review screen.
