# NMS Social Reports

A lightweight browser-based social media analytics dashboard for National Model School accounts.

## Features
- Import Meta exports as Excel (.xlsx/.xls) or CSV
- KPI summary for views, reach, engagements and average hook rate
- Trend, content mix, account comparison and hook-vs-hold charts
- Filter by account, content type and date range
- Search/sort posts and switch between table and card views
- Manually enter hook and hold rates per post
- Export the imported data and manual rates to CSV
- Responsive layout using NMS navy/yellow/white branding

## Run
Open `index.html` in a modern browser, or publish it using GitHub Pages.

## Publish with GitHub Pages
1. Open the repository's **Settings**.
2. Choose **Pages** in the sidebar.
3. Under Build and deployment, choose **Deploy from a branch**.
4. Select branch `main` and folder `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site; the URL will be shown on the Pages settings screen.

## Data storage note
This initial version saves imported posts and manually entered rates in the current browser using local storage. It does **not** write data to Google Sheets yet, and data is not automatically shared across browsers or devices. Importing a new report replaces the currently loaded dataset in this browser. Export CSV to keep a portable copy.

## Expected import columns
The importer tries to recognize common Meta column headings for date, account/page, post/caption, post link, content type, views, reach, engagements, hook rate, hold rate, and video duration. The first row should contain headers.
