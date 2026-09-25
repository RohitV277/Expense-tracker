# 💶 Expense Tracker Dashboard

A personal expense dashboard — charts, filters, search, and a live ledger — hosted as a free static site and backed by a Google Sheet as the database.

<img src="https://img.shields.io/badge/hosted%20on-GitHub%20Pages-4A86E8?logo=github" alt="GitHub Pages">
<img src="https://img.shields.io/badge/backend-Google%20Apps%20Script-34A853?logo=googlesheets&logoColor=white" alt="Google Apps Script">
<img src="https://img.shields.io/badge/data-Google%20Sheets-0F9D58?logo=googlesheets&logoColor=white" alt="Google Sheets">

## ✨ What this is

This page (`index.html`) is a **view**, not a database. All your actual expense data lives in a Google Sheet. This site talks to that sheet through a small Google Apps Script API, so:

- 📊 Filter by date range, category, payment mode, or bank/card
- 🔍 Search remarks, category, or bank/card
- ➕ Add, ✏️ edit, and 🗑️ delete expenses from your phone or tablet
- 📱 Installs like a real app via **Add to Home Screen** on iPhone/iPad

## 🚀 Setup

1. Open `index.html`, find the line near the top of the `<script>` tag:
   ```js
   const API_BASE_URL = 'PASTE_YOUR_APPS_SCRIPT_WEB_APP_URL_HERE';
   ```
   Replace it with your own Apps Script Web App URL (ends in `/exec`).
2. Push this repo to GitHub, then enable **Settings → Pages** (see full steps below).
3. Open the resulting `github.io` link on your phone, then **Share → Add to Home Screen**.

## 🗂️ Files in this repo

| File | Purpose |
|---|---|
| `index.html` | The whole app — dashboard UI + the API layer that talks to your Google Sheet |
| `favicon.ico` | Browser tab icon |

## ⚠️ Note

This repo only contains the frontend. The backend (`Code.gs` + `Dashboard.html`) lives in your Google Sheet's Apps Script project, not here.
