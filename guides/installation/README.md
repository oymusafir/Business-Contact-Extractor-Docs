# Business Contact Extractor Installation Guide

Follow this guide to install **Business Contact Extractor v1.5.0** in Google Chrome on Windows or macOS.

## Before you begin

You need:

- A Windows or macOS computer
- The desktop version of Google Chrome
- The Business Contact Extractor ZIP file
- A valid licence key
- An internet connection

Business Contact Extractor does not run in mobile Chrome on Android, iPhone, or iPad.

## Important folder rule

After extracting the ZIP file, the extension folder must be named:

```text
Business Contact Extractor
```

Keep this folder in a permanent location. Chrome runs the extension directly from it. Moving, renaming, or deleting the folder can stop the extension from working.

Recommended locations:

### Windows

```text
Documents\Blaster Pro Tools\Business Contact Extractor
```

### macOS

```text
Documents/Blaster Pro Tools/Business Contact Extractor
```

Avoid keeping the installed folder inside Downloads, a temporary folder, a removable drive, or a cloud folder that automatically removes local files.

## 1. Extract the ZIP file

Chrome cannot install the extension directly from a ZIP file.

### Windows

1. Find the downloaded ZIP file.
2. Right-click it and choose **Extract All**.
3. Move the extracted folder to your permanent location.
4. Confirm the folder is named `Business Contact Extractor`.
5. Open the folder.

### macOS

1. Find the downloaded ZIP file in Finder.
2. Double-click it to extract it.
3. Move the extracted folder into Documents or another permanent location.
4. Confirm the folder is named `Business Contact Extractor`.
5. Open the folder.

## 2. Confirm the correct folder

The `Business Contact Extractor` folder must directly contain:

```text
manifest.json
```

It should also contain extension folders such as:

```text
assets
background
dashboard
offscreen
popup
scraper
website-scanner
```

If you open `Business Contact Extractor` and find another folder with the same name inside it, open the inner folder. Select the folder that directly contains `manifest.json` when Chrome asks you to load the extension.

## 3. Open Chrome Extensions

Open Google Chrome and enter:

```text
chrome://extensions
```

Press Enter.

You can also open:

```text
Chrome menu > Extensions > Manage Extensions
```

## 4. Enable Developer mode

Turn on **Developer mode** in the top-right corner of the Chrome Extensions page.

Chrome will display additional buttons, including **Load unpacked**.

## 5. Load Business Contact Extractor

1. Select **Load unpacked**.
2. Browse to the permanent `Business Contact Extractor` folder.
3. Select the folder that directly contains `manifest.json`.
4. Confirm the selection.

Chrome should now show an extension card named:

```text
Extractor by Blaster Pro Tools
```

Confirm that:

- the extension is enabled;
- the displayed version is `1.5.0`; and
- no error appears on the extension card.

Chrome may display a developer-mode warning because the extension is installed directly instead of through the Chrome Web Store. This is expected.

## 6. Pin the extension

1. Select the Extensions icon in the Chrome toolbar.
2. Find **Extractor by Blaster Pro Tools**.
3. Select the pin icon.

The Extractor icon should remain visible in the toolbar.

## 7. Activate your licence

1. Select the Extractor icon.
2. Wait while the extension checks for an existing licence.
3. Enter your licence key.
4. Enter your name, phone number, email address, and city.
5. Select **Activate**.
6. Wait for the successful activation message.

The licence is connected to the current Business Contact Extractor installation and Chrome profile. Internet access is required for activation and subscription validation.

If the licence was previously activated in another Chrome profile or computer, request a reset before activating it again. Read [Licence Activation and Device Transfer](../licence-and-device-transfer/README.md).

## 8. Select the correct country

Before collecting or scanning phone numbers:

1. Open Extractor.
2. Choose the country where your target businesses are located.
3. Confirm the displayed international calling code.
4. Enable local-number conversion only when the results contain local phone formats.

The selected country helps Extractor reject dates, IDs, short number fragments, impossible numbers, and numbers belonging to a different country.

If your search targets another country, update the country selection before collecting the new results.

## 9. Test Google collection

1. Open a normal Google search results page.
2. Search for a business category and location, for example:

```text
boutiques in Dubai
```

3. Wait until the results finish loading.
4. Open Extractor.
5. Select **Collect This Page**.
6. Open the contacts dashboard.

The dashboard should show any recognizable public business names, phone numbers, WhatsApp links, emails, websites, and source links found in the visible results.

Not every Google result contains usable contact information. Try a focused query from the [Google Search Query Handbook](../search-queries/README.md) if the first search produces few contacts.

## 10. Test the Website Scanner

The Website Scanner uses optional website access permission to check the public business websites you select.

1. Open the Website Scanner.
2. Select the correct country.
3. Add a public business website or choose contacts from your saved list.
4. Choose a reasonable delay.
5. Start the scan.
6. Approve Chrome's website permission request.

The scanner may check a limited number of relevant pages such as contact, about, support, or help pages. New public contact details are merged into the existing list.

Website results depend on what the website publishes and allows Chrome to request. Login pages, CAPTCHAs, image-only contacts, JavaScript-only content, and security services may prevent scanning.

Read the complete [Website Contact Scanner Guide](../website-scanner/README.md).

## 11. Update safely

Keep the installed folder name and location unchanged:

```text
Business Contact Extractor
```

Recommended update process:

1. Export important contacts to CSV or JSON.
2. Close the Extractor popup and dashboard.
3. Download the new official update ZIP.
4. Extract the update into a temporary location.
5. Copy the new files into the existing `Business Contact Extractor` folder.
6. Allow the new files to replace the previous extension files.
7. Open `chrome://extensions`.
8. Find **Extractor by Blaster Pro Tools**.
9. Select the reload icon.
10. Open Extractor and confirm the new version.

Do not rename the installed folder for each version. The permanent folder remains `Business Contact Extractor`.

## 12. Move to another computer or Chrome profile

Before moving:

1. Export important contacts to CSV or JSON.
2. Keep your licence key available.
3. Request a licence reset from Blaster Pro Tools.
4. Install the extension on the destination computer or Chrome profile.
5. Keep the destination folder named `Business Contact Extractor`.
6. Activate the same valid licence after the reset.

A reset removes the previous installation binding. It does not change the subscription expiration date.

## 13. Uninstall

Before uninstalling, export any contacts you want to keep.

To remove the extension:

1. Open `chrome://extensions`.
2. Find **Extractor by Blaster Pro Tools**.
3. Select **Remove**.
4. Confirm the removal.

Chrome may delete locally stored contacts and activation information when the extension is removed. Removing the extension does not automatically reset the licence binding. Contact Blaster Pro Tools if you want to activate it elsewhere.

After confirming that your exports are safe and the extension is removed, you may delete the `Business Contact Extractor` folder.

## Common installation problems

### Load unpacked is missing

Developer mode is not enabled. Open `chrome://extensions` and turn on **Developer mode**.

### Manifest file is missing or unreadable

The wrong folder was selected or the ZIP was not extracted correctly.

Select the `Business Contact Extractor` folder that directly contains:

```text
manifest.json
```

### Service worker registration failed, status code 15

One or more extension files are missing, incomplete, or damaged.

1. Remove the failed extension card.
2. Extract a fresh official ZIP.
3. Confirm the complete folder structure is present.
4. Load the `Business Contact Extractor` folder again.

### Licence key not found

Check the licence key carefully. Avoid extra spaces and confirm every letter and number. Contact Blaster Pro Tools if the same message continues.

### Licence already activated elsewhere

The licence is still connected to another installation. Request a licence reset before trying again.

### Could not connect to the licence service

Check:

- the internet connection;
- firewall or security software;
- computer date, time, and timezone; and
- whether the support service is reachable.

Then select **Retry validation**.

### Open a Google search results page first

Open a normal Google web search, wait for the visible results to load, and reopen Extractor. Google Maps, Images, Shopping, and other specialized pages may use different layouts.

### No contacts were collected

Confirm the correct country is selected and inspect whether the visible Google snippets actually contain public contact information. Use a more focused query and try again.

### Website scanning does not start

Confirm that:

- the licence is active;
- the URL is a public `http` or `https` business website;
- website permission was granted;
- the country is selected; and
- the website opens normally in Chrome.

### Saved contacts disappeared

Chrome may remove extension storage after uninstalling, changing profiles, or clearing browser data. Restore the information from your latest CSV or JSON export.

## Installation checklist

- [ ] The ZIP file is extracted
- [ ] The permanent folder is named `Business Contact Extractor`
- [ ] The folder directly contains `manifest.json`
- [ ] Developer mode is enabled
- [ ] The extension was loaded with **Load unpacked**
- [ ] Extractor shows version `1.5.0`
- [ ] The extension is enabled and pinned
- [ ] The licence is active
- [ ] The correct country is selected
- [ ] Google collection was tested
- [ ] Website permission was approved when needed
- [ ] Important contacts are exported before updates or removal

## Need help?

Read [Troubleshooting](../troubleshooting/README.md) or visit [Blaster Pro Tools](https://blasterprotools.com/).

When requesting help, include the Extractor version, operating system, Chrome version, exact error message, and a screenshot with sensitive information hidden.

## Responsible use

Collect only relevant contact information that businesses have made public. Follow applicable privacy, marketing, anti-spam, platform, and telecommunications rules before contacting any business.
