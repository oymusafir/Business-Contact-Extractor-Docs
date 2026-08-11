# Website Contact Scanner

The Website Contact Scanner checks selected public business websites for phone numbers, WhatsApp links, email addresses, and useful contact pages. Its results are merged into the same contact records collected from Google.

## When to use it

Use the scanner after Google collection when a record:

- has an email but no phone number;
- has a phone number but no email;
- has only a personal email and you want to look for a business-domain email;
- includes a business website that may contain additional public contacts; or
- needs a clearer source for the contact information.

## Before scanning

1. Open the website scanner from Extractor.
2. Grant the optional website access permission when Chrome asks. The scanner needs this permission to request the public pages you select.
3. Select the correct country and calling code. Country-based validation helps reject unrelated numbers, dates, order IDs, and broken number fragments.
4. Choose a reasonable delay between requests. A slower delay is more respectful and can reduce temporary blocking.
5. Select existing contacts or add business website URLs, one URL per line.

## How a scan works

1. Extractor requests the public website page without signing in.
2. It reads visible HTML and public contact links such as `mailto:`, `tel:`, and WhatsApp links.
3. It may follow a limited number of same-site pages whose labels suggest contact, about, support, help, or customer service information.
4. Email addresses are cleaned, classified, and deduplicated.
5. Phone candidates are validated against the selected country before they are saved.
6. New details are merged with the existing contact instead of creating unnecessary duplicates.

## Email behavior

- Business-domain emails are useful when the domain belongs to the business website.
- Personal providers such as Gmail, Yahoo, Outlook, Hotmail, and Live are categorized separately.
- Additional emails remain available when the website publishes more than one valid address.
- Extractor rejects many joined labels, copied captions, image filenames, malformed domains, and text accidentally attached after common personal email domains.
- No automatic cleaner can understand every badly structured website. Review important records before outreach.

## Phone behavior

- The selected country and calling code determine which numbers are accepted.
- International numbers should include `+` or `00` when displayed on a website.
- Local numbers can be converted when local conversion is enabled and the country is selected correctly.
- Possible but invalid numbers should not be saved as contacts.
- WhatsApp links are identified separately when the website provides them.

## Why a website may return no contacts

The scanner may not find contacts when:

- the site requires a login;
- the contact information is inside an image, video, PDF, or protected widget;
- the page is rendered entirely by JavaScript after loading;
- a firewall, anti-bot service, or security policy blocks extension requests;
- the website returns an error or redirects unexpectedly;
- the contact information is not publicly displayed; or
- the selected country does not match the site's phone numbers.

An empty result does not mean the extension is broken. Open the source website manually and confirm that the contact details are visible as normal page text.

## Responsible scanning

Scan only relevant public business websites. Use a reasonable delay, avoid excessive repeated requests, and respect the website's terms and applicable law. Extractor is not designed to bypass logins, CAPTCHAs, paywalls, access controls, or private pages.

For permission and scanning errors, see [Troubleshooting](../troubleshooting/README.md).
