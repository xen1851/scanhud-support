# Privacy Policy for ScanHUD

**Last Updated:** January 28, 2026

**ScanHUD** ("we", "our", or "the extension") is a developer tool designed to extract text from browser content using Optical Character Recognition (OCR). We take user privacy seriously. This policy explains how ScanHUD handles data.

## 1. No Data Collection
ScanHUD does not collect, transmit, or sell personal information.

* We **do not** use analytics, tracking, advertising, or telemetry services.
* We **do not** collect browsing history or monitor pages in the background.
* ScanHUD only operates on the active browser tab when **explicitly triggered by the user**.

## 2. Local OCR Processing
All OCR processing is performed **locally on your device**.

* When you select an area to scan, a temporary screenshot of that area is created in the browser’s memory.
* The image is processed locally using **Tesseract.js** (WebAssembly).
* **No images, extracted text, or metadata are uploaded to any external server.**
* Once processing is complete, the image data is discarded from memory.

## 3. Local Storage
ScanHUD stores limited data locally on your device:

* **Recent scan history** (extracted text and timestamps) is saved using `chrome.storage.local`.
* This data remains on your machine and is not synced to Google servers or accessible by us.
* You can clear this data at any time via the extension settings or by clearing browser extension data.

## 4. Permissions Usage
ScanHUD requires the following browser permissions to function:

* **`activeTab`**: Used only after explicit user interaction (clicking the extension icon or button) to capture the visible area of the current tab for OCR.
* **`scripting`**: Used to inject a lightweight selection overlay (HUD) into the active page so the user can choose the scan area.
* **`offscreen`**: Used to run the OCR engine in an isolated offscreen context to avoid blocking or slowing down the main browsing experience.
* **`storage`**: Used to store scan history and user preferences locally on the device.

## 5. Third-Party Libraries
ScanHUD uses **Tesseract.js**, an open-source OCR engine.

* Tesseract.js is bundled with the extension and executed locally.
* It does not transmit data externally or communicate with third-party services.

## 6. Contact
If you have questions about this Privacy Policy or ScanHUD’s data handling practices, please contact us via our email:

alex.stelmakh@protonmail.com
