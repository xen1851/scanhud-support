Last Updated: March 10, 2026

ScanHUD (“we”, “our”, or “the extension”) is a developer tool designed to extract and analyze technical text (such as logs or console output) directly from the screen using Optical Character Recognition (OCR). We take user privacy seriously. This policy explains how ScanHUD handles data.


# 1. No Personal Data Collection

ScanHUD does not collect, store, sell, or share personal information.

We do not use:

- advertising networks
    
- tracking services
    
- behavioral analytics
    
- background monitoring of browsing activity
    

The extension only operates on the active browser tab when explicitly triggered by the user.


# 2. Local OCR Processing

All OCR processing is performed locally on your device.

When you select an area to scan:

- a temporary screenshot of the selected region is created in the browser’s memory
    
- the image is processed locally using **Tesseract.js (WebAssembly)**
    
- extracted text is generated locally in the browser
    

No screenshots, extracted text, or metadata are uploaded to external servers.

Once processing is complete, the image data is discarded from memory.


# 3. Optional AI Analysis (BYOK)

ScanHUD provides an optional AI analysis feature to help interpret extracted text such as logs or error messages.

This feature uses a **Bring Your Own Key (BYOK)** model:

- users may optionally provide their own **OpenAI API key**
    
- AI analysis is performed by sending selected text directly to the **OpenAI API**
    
- ScanHUD does not proxy, store, or process these requests on its own servers
    

Only the text explicitly chosen by the user for analysis is sent to the OpenAI API.

Users are responsible for reviewing and complying with the **OpenAI Privacy Policy and Terms of Service** when using this feature.

AI analysis is entirely optional and disabled unless the user explicitly configures an API key.


# 4. Local Storage

ScanHUD stores limited data locally on the user’s device.

This may include:

- recent scan history (extracted text and timestamps)
    
- extension settings and preferences
    
- user-provided OpenAI API key (if configured)
    

This information is stored using `chrome.storage.local` and remains on the user's device.

ScanHUD does not sync this data to external servers.

Users can clear this data at any time through extension settings or by clearing browser extension data.


# 5. Permissions Usage

ScanHUD requires the following browser permissions:

**activeTab**  
Used only after explicit user interaction to capture the visible area of the active tab for OCR.

**scripting**  
Used to inject a lightweight overlay interface (HUD) so the user can select the area to scan.

**offscreen**  
Used to run the OCR engine in an isolated context to avoid blocking the main browser thread.

**storage**  
Used to store local preferences, scan history, and optional API key configuration.


# 6. Third-Party Components

ScanHUD includes the following third-party components:

**Tesseract.js**  
Open-source OCR engine bundled with the extension and executed locally.

**OpenAI API (optional)**  
Used only when the user enables AI analysis and provides their own API key.

ScanHUD does not operate or manage any backend service for AI processing.


# 7. Contact

If you have questions about this Privacy Policy or ScanHUD’s data handling practices, please contact:

alex.stelmakh@protonmail.com
