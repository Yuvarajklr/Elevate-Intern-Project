# 🔐 Malicious Firefox Extension Removal Project

## 📅 Date: 04 July 2025

## 📌 Objective
Identify, analyze, and remove malicious or suspicious extensions from the Firefox browser to improve privacy and security.

---

## 🧭 Steps Taken

### 1. Accessed Firefox Extension Manager
- Navigated to: `Menu → Add-ons and Themes → Extensions`
- Reviewed all currently installed extensions.

### 2. Identified Suspicious Extensions
**Evaluation criteria:**
- Unknown or rarely used extensions.
- Poor user ratings and limited reviews on the Mozilla Add-ons site.
- Excessive or unnecessary permissions.
- Unusual browser behavior (ads, redirects, slowness).

### 3. Verified Extensions Online
- Looked up extensions on:
  - [addons.mozilla.org](https://addons.mozilla.org/)
  - Google for reputation reports or discussions.
- Uploaded `.xpi` files to [VirusTotal](https://www.virustotal.com) for malware analysis.

### 4. Manual Inspection of Extensions
- Located `.xpi` files from the Firefox profile directory.
- Unzipped and reviewed:
  - `manifest.json` for permissions
  - `.js` files for obfuscated code or malicious behavior

### 5. Removed Malicious Extensions
- Used Firefox's built-in Remove option for untrusted extensions.

---

## ❌ Removed Extensions

| Extension Name          | Reason for Removal                                | Detection Method            | Status   |
|-------------------------|----------------------------------------------------|-----------------------------|----------|
| EasyPDFCombine          | Redirects to fake search engines                  | VirusTotal, User Reports   | ✅ Removed |
| Video Downloader Pro    | Injected ads into webpages                        | Manual Analysis             | ✅ Removed |
| Weather Forecast Plus   | Requested tracking permissions unnecessarily      | Review + Manifest.json      | ✅ Removed |
| Search Manager          | Hijacked default search provider                  | Browser Behavior            | ✅ Removed |
| SaveFrom Helper         | Detected malware behavior                         | VirusTotal                  | ✅ Removed |

---

## 🛡️ Post-Cleanup Actions
- Restarted Firefox browser.
- Verified clean list of extensions.
- Ran malware scan with:
  - **Windows Defender**
  - **Malwarebytes**
- Reset Firefox settings (optional but recommended).

---

## ✅ Final Status
- All known malicious/suspicious extensions have been removed.
- Browser behavior returned to normal.
- No further signs of infection or hijacking.

---
