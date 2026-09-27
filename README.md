# Sri Mahalaxmi · Boutique and Zari Works

The shop website for Sri Mahalaxmi, Nizamabad. Customers browse sarees in stock and enquire on WhatsApp.

## How it works

- **Stock lives in a private Google Sheet.** The family updates it from the Google Sheets app on their phones.
- **The website reads the sheet's Stock tab** every time someone opens it, so it is always up to date. Nothing needs to be changed here for day-to-day stock updates.
- Cost prices and sales stay in the sheet's private tab and never reach this website.

## One-time setup

1. Import `Sri-Mahalaxmi-Stock.xlsx` into Google Sheets (Google Drive → New → File upload, then open it with Google Sheets).
2. In the sheet: **File → Share → Publish to web**, choose the **Stock** tab and **Comma-separated values (.csv)**, then **Publish**. Copy the link.
3. In this repository, edit `index.html`, find `sheetCsvUrl: ""` near the top and paste the link between the quotes. Commit.

Until step 3 is done, the site reads `stock.csv` in this repository.

## Changing shop details

Name, tagline, city and WhatsApp number are in the `window.SHOP` block at the top of `index.html`.
