# Troubleshooting

Use this page to solve the most common Business Contact Extractor problems. Start with the exact message shown by Chrome or the extension.

## Quick fixes

| Problem | Likely cause | What to do |
| --- | --- | --- |
| Load unpacked is missing | Developer mode is off | Open `chrome://extensions` and enable **Developer mode** |
| Manifest file is missing or unreadable | The wrong folder was selected or the ZIP is still compressed | Extract the ZIP and select the `Business Contact Extractor` folder that directly contains `manifest.json` |
| Service worker registration failed, status code 15 | A background file is missing, invalid, or damaged | Extract fresh official Business Contact Extractor files and reload the extension |
| Extension icon is missing | Assets were moved or the package is incomplete | Restore the original folder structure or reinstall from a clean ZIP |
| Licence key not found | The key was entered incorrectly or was not issued | Re-enter it carefully and confirm it with support |
| Licence is active elsewhere | The key is bound to another installation | Request a licence reset before activating again |
| Licence server cannot be reached | Internet, firewall, DNS, date, or time problem | Check the connection and system clock, then retry |
| Activation disappeared after an update | The extension was removed, loaded from a different folder, or profile data was cleared | Request a reset if the installation identity changed |
| Open a Google search results page first | The active tab is not a standard Google results page | Open a normal Google web search, wait for results, and reopen Extractor |
| Zero contacts collected | The visible results contain no recognizable public contacts or the query is too broad | Try a focused query and inspect the visible snippets |
| Some visible numbers are not collected | The number is invalid for the selected country, duplicated, or not represented as a contact | Confirm the country and calling code, then collect again |
| Website permission was denied | Chrome did not grant access to public websites | Start the scanner again and approve the permission prompt |
| Website returned no contacts | Contacts are hidden, dynamically rendered, protected, or absent | Open the website manually and check its contact page |
| Website request is blocked | The site's CORS, firewall, anti-bot, or access rules rejected the request | Skip that site or collect the visible public details manually |
| Contacts disappeared after uninstalling | Chrome removed the extension's local storage | Restore from a CSV or JSON export if one was created |

## Installation checks

1. Confirm the package is extracted, not opened inside the ZIP viewer.
2. Confirm `manifest.json` is directly inside the selected `Business Contact Extractor` folder.
3. Confirm the complete `Business Contact Extractor` folder remains in a permanent location.
4. Open `chrome://extensions` and inspect the error button on the Extractor card.
5. If the package was built from source, run the official test and build commands before loading `dist`.

Read the complete [Installation Guide](../installation/README.md).

## Collection checks

1. Use a standard Google web results page.
2. Wait until the result cards have finished loading.
3. Confirm the correct country and calling code.
4. Collect the current page only once, then move to the next page.
5. Try a query from the [Google Search Query Handbook](../search-queries/README.md).
6. Remember that Extractor only saves contacts it can identify in the visible result content and public links.

## Website scanner checks

1. Confirm the row contains a real business website, not a social network, Google page, or WhatsApp link.
2. Open the website manually and verify it loads.
3. Confirm website permission was granted.
4. Confirm the selected country matches the business location.
5. Increase the delay if several websites are being scanned.
6. Read [Website Contact Scanner](../website-scanner/README.md) for limitations.

## Before contacting support

Prepare:

- the exact error message;
- a screenshot of the extension card or popup;
- Chrome version and operating system;
- Extractor version;
- the action you performed immediately before the error;
- one example search query or public website URL, if relevant; and
- confirmation that you tested a fresh official package.

Do not send passwords, cookies, complete payment card details, or private customer lists.

See [Support](../../SUPPORT.md) for contact details.
