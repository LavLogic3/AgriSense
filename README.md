# AgriSense — Earth & Terracotta Edition

A responsive, browser-based agriculture intelligence prototype built with HTML, CSS and vanilla JavaScript.

## Run locally in VS Code
1. Extract this ZIP file.
2. Open the extracted `AgriSense_Earth_Terracotta` folder in Visual Studio Code.
3. Open `index.html` in a browser, or use the **Live Server** extension and choose **Open with Live Server**.

No build step, Node.js installation, API key or database is required.

## Features
- **Farm Passport:** Save farm name, owner, location, area, soil type, main crop and planting date.
- **Crop Scanner:** Upload a crop photo and view simple colour-pattern estimates.
- **Crop Health Timeline:** Save scan results locally and view a visual trend chart.
- **PDF Reports:** Export individual observation reports using the browser print dialog; select **Save as PDF**.
- **Full-site language switch:** English, Hindi and Telugu translations apply to navigation, page headings, forms, helper text, empty states, status messages and report content.
- Responsive layout with an Earth & Terracotta colour palette.

## Important technical notes
- Farm profile and scan history are stored in the browser's `localStorage` on the current device/browser. They are not synced to other devices.
- The crop scanner uses a basic image-colour heuristic (green/yellow/dark/brown pixel proportions). It is **not** a trained AI model and cannot diagnose plant disease.
- The PDF export opens a print-ready report in a new browser tab. In the print dialog, choose **Save as PDF**.
- Google Fonts are used when an internet connection is available; system fallbacks are provided.

## Files
- `index.html` — page structure
- `style.css` — layout, palette and responsive styles
- `app.js` — translations, farm profile, scan analysis, timeline and report export
