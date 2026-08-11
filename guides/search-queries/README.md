# Google Search Query Handbook

Practical Google search training for Business Contact Extractor customers.

This handbook explains how to build focused Google searches for finding publicly available business websites, contact pages, email signals, WhatsApp pages and social profiles.

You do not need advanced operators for every search. A normal search such as `boutiques in Dubai` may already produce useful results. Use the operators in this handbook only when you need to narrow, clean or improve those results.

> Search operators are filters, not magic commands. Google still decides which indexed pages are relevant enough to display. Always review and verify every result before using it.

## Table of contents

1. [How Google reads a query](#1-how-google-reads-a-query)
2. [The five parts of a useful business query](#2-the-five-parts-of-a-useful-business-query)
3. [Exact phrase searches](#3-exact-phrase-searches)
4. [Search a website, platform or country domain with site](#4-search-a-website-platform-or-country-domain-with-site)
5. [Remove unwanted results](#5-remove-unwanted-results)
6. [Search for alternatives with OR](#6-search-for-alternatives-with-or)
7. [Find business email signals](#7-find-business-email-signals)
8. [Control URL patterns with inurl](#8-control-url-patterns-with-inurl)
9. [Search by date with after and before](#9-search-by-date-with-after-and-before)
10. [Keep words close with AROUND](#10-keep-words-close-with-around)
11. [How to combine operators correctly](#11-how-to-combine-operators-correctly)
12. [Copy-ready query templates](#12-copy-ready-query-templates)
13. [A realistic search workflow](#13-a-realistic-search-workflow)
14. [Troubleshooting poor results](#14-troubleshooting-poor-results)
15. [Quick reference](#15-quick-reference)

---

## 1. How Google reads a query

Google does not search the live internet every time you press Enter. It searches pages that Google has already discovered, processed and added to its index.

When you enter a query, Google tries to understand:

- The subject you want
- The location you are targeting
- The type of page you may prefer
- The exact words or phrases that matter
- The words, websites or URL patterns you want removed
- Whether the freshness of the page matters

For example:

```text
"boutique" "Dubai" ("email" OR "WhatsApp") -jobs -careers -hiring
```

Google can read this as:

- Find pages related to the exact word `boutique`
- Keep `Dubai` relevant to the result
- Accept pages mentioning either `email` or `WhatsApp`
- Remove pages focused on jobs, careers or hiring

The operators improve the request, but they do not guarantee that every matching page will appear. Some public pages are not indexed, some pages are outdated, and Google may ignore or relax parts of a complicated query.

### Start with a normal search

Before adding operators, try a simple query:

```text
boutiques in Dubai
```

Review the first page and ask:

- Are the results actually boutiques?
- Are they located in Dubai?
- Are Google results showing websites, social profiles or directories?
- Are contact details visible in titles or descriptions?
- Which words do these businesses use to describe themselves?

The first search teaches you the market vocabulary. You can then build a better query using the words businesses actually use.

---

## 2. The five parts of a useful business query

A practical business search normally contains up to five parts.

### 1. Business category

What kind of business do you want?

Examples:

- Boutique
- Dentist
- Real estate agency
- Accounting firm
- Commercial cleaning company
- Marketing agency
- Restaurant
- Construction contractor

Placeholder:

```text
[CATEGORY]
```

### 2. Location

Where should the business operate?

Examples:

- Dubai
- Abu Dhabi
- Houston
- London
- Toronto
- New York
- Texas
- United Arab Emirates

Placeholder:

```text
[LOCATION]
```

### 3. Contact signal

What type of information should the page mention?

Examples:

```text
"contact"
```

```text
("email" OR "WhatsApp")
```

```text
("info@" OR "contact@" OR "sales@" OR "hello@")
```

### 4. Source

Should results come from a particular website, platform or country domain?

Examples:

```text
site:wa.me
```

```text
site:instagram.com
```

```text
site:linkedin.com/company
```

```text
site:.ae
```

### 5. Exclusions

What kind of noise should be removed?

Examples:

```text
-jobs -careers -hiring
```

```text
-site:facebook.com -site:instagram.com -site:linkedin.com
```

```text
-inurl:reel -inurl:p
```

### The master query

This is a reliable starting structure:

```text
"[CATEGORY]" "[LOCATION]" "contact" -site:facebook.com -site:instagram.com -site:linkedin.com
```

Example:

```text
"commercial cleaning" "Abu Dhabi" "contact" -site:facebook.com -site:instagram.com -site:linkedin.com
```

Do not add every available operator at once. Start with the category and location, then add one new filter at a time.

---

## 3. Exact phrase searches

### Syntax

```text
"exact phrase"
```

Quotation marks tell Google that the enclosed words should stay together as a phrase.

### Without quotation marks

```text
real estate agency Dubai
```

Google may match pages containing variations of these words in different places.

### With quotation marks

```text
"real estate agency" "Dubai"
```

This asks Google to keep `real estate agency` together and also keep `Dubai` relevant.

### Good uses

Use quotation marks for:

- Business categories with multiple words
- Exact cities or regions
- Contact phrases
- Known business names
- Specific services

Examples:

```text
"digital marketing agency" "New York"
```

```text
"commercial cleaning" "Abu Dhabi"
```

```text
"dental clinic" "Houston" "contact"
```

```text
"Noor Boutique" "Dubai"
```

### Common mistake

Do not quote an entire long sentence:

```text
"find me all boutique businesses in Dubai with email and WhatsApp"
```

Few pages will contain that complete sentence, so the search may return nothing.

Use separate meaningful phrases instead:

```text
"boutique" "Dubai" ("email" OR "WhatsApp")
```

---

## 4. Search a website, platform or country domain with site

### Syntax

```text
site:domain.com
```

The `site:` operator requests results from a particular domain, website or URL prefix.

There must be no space after `site:`.

Correct:

```text
site:instagram.com "boutique" "Dubai"
```

Incorrect:

```text
site: instagram.com "boutique" "Dubai"
```

### Search one website

```text
site:example.com ("email" OR "WhatsApp")
```

Replace `example.com` with the actual domain you want to inspect.

### Search WhatsApp business pages

```text
site:wa.me "boutique" "Dubai"
```

```text
site:wa.me "restaurant" "Toronto"
```

```text
site:wa.me "real estate" "London"
```

These queries look for indexed `wa.me` pages related to the selected category and location.

### Search Instagram profiles

```text
site:instagram.com "boutique" "Dubai" ("email" OR "WhatsApp")
```

Instagram results may include profiles, posts and reels. Later in this handbook, you will learn how to reduce post and reel URLs.

### Search LinkedIn company pages

```text
site:linkedin.com/company "software agency" "Texas"
```

```text
site:linkedin.com/company "accounting firm" "Dubai" ("email" OR "contact")
```

Using `/company` focuses the query more closely on company pages instead of personal profiles.

### Search Facebook pages

```text
site:facebook.com "restaurant" "Houston" ("email" OR "WhatsApp")
```

Facebook may limit what Google can index, so results can vary.

### Search UAE domains

```text
site:.ae "interior design" "Dubai"
```

```text
site:.ae "accounting firm" "Abu Dhabi" "contact"
```

```text
site:.ae "commercial cleaning" ("info@" OR "contact@")
```

`site:.ae` focuses on indexed websites using the UAE `.ae` domain ending. It will not include every UAE business because many UAE businesses use `.com`, `.net` or other domain endings.

### Important limitation

`site:` results are not an exact count of every indexed page. Treat them as a useful result sample, not a complete database.

---

## 5. Remove unwanted results

The minus sign removes words, phrases, websites or URL patterns.

There must be no space after the minus sign.

### Remove individual words

```text
-jobs -careers -hiring
```

Example:

```text
"marketing agency" "New York" "contact" -jobs -careers -hiring
```

This reduces recruitment pages when your goal is business contact information.

### Remove an exact phrase

```text
-"job vacancy"
```

Example:

```text
"construction company" "Dubai" "contact" -"job vacancy"
```

### Remove entire websites

```text
-site:facebook.com -site:instagram.com -site:linkedin.com
```

Example:

```text
"boutique" "Dubai" "contact" -site:facebook.com -site:instagram.com -site:linkedin.com
```

Use this when social profiles are dominating the results and you want more official business websites, directories or contact pages.

### Remove shopping and marketplace noise

```text
-amazon -etsy -ebay -walmart
```

Example:

```text
"jewelry boutique" "Texas" "contact" -amazon -etsy -ebay -walmart
```

### Do not overuse exclusions

Every exclusion can hide useful results. If the query becomes weak, remove exclusions one at a time.

Bad approach:

```text
"boutique" "Dubai" -jobs -careers -hiring -shop -store -fashion -clothing -instagram -facebook -linkedin
```

This removes words that may be important to the business itself.

Better approach:

```text
"boutique" "Dubai" "contact" -jobs -careers -hiring
```

---

## 6. Search for alternatives with OR

`OR` tells Google that either alternative is acceptable.

Keep `OR` uppercase.

### Basic syntax

```text
"email" OR "WhatsApp"
```

### Recommended grouped syntax

```text
("email" OR "WhatsApp")
```

Parentheses keep the alternatives together and make longer queries easier to understand.

### Contact signal example

```text
"boutique" "Dubai" ("email" OR "WhatsApp")
```

The result can qualify when it contains either `email` or `WhatsApp`.

### Category alternatives

```text
("boutique" OR "fashion store" OR "clothing store") "Dubai" "contact"
```

This is useful when the same business type uses different names.

### Location alternatives

```text
"accounting firm" ("Dubai" OR "Abu Dhabi") "contact"
```

### Combined alternatives

```text
("boutique" OR "fashion store") ("Dubai" OR "Abu Dhabi") ("email" OR "WhatsApp")
```

This query is broader because any category, location and contact alternative can match.

### Common mistakes

Do not use lowercase `or`:

```text
"email" or "WhatsApp"
```

Google may treat lowercase `or` as a normal word.

Do not forget parentheses in a long query:

```text
"boutique" "Dubai" "email" OR "WhatsApp" -jobs
```

The meaning becomes less clear. Use:

```text
"boutique" "Dubai" ("email" OR "WhatsApp") -jobs
```

---

## 7. Find business email signals

Many businesses publish role-based email addresses such as:

- `info@company.com`
- `contact@company.com`
- `sales@company.com`
- `hello@company.com`
- `support@company.com`
- `admin@company.com`

A useful Google query searches for the beginning of these addresses.

### Core business email group

```text
("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Search business emails by category and location

```text
"real estate agency" "Dubai" ("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Focus on UAE websites

```text
site:.ae "real estate" "Dubai" ("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Exclude job pages

```text
"marketing agency" "New York" ("info@" OR "contact@" OR "sales@" OR "hello@") -jobs -careers -hiring
```

### Search a known domain

```text
site:example.com ("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Search both business and general email words

```text
"accounting firm" "London" ("info@" OR "contact@" OR "sales@" OR "hello@" OR "email")
```

### What this query does not prove

Finding an email string does not automatically prove that:

- The address is active
- The address belongs to the business in the title
- The result is current
- The business accepts promotional messages
- The address is the best contact for your offer

Always open the source and confirm the business identity before using the result.

---

## 8. Control URL patterns with inurl

`inurl:` requests pages whose URL contains a particular word or pattern.

This operator can be useful, but it is less consistent than exact phrases, `site:`, exclusions and date operators. Use it as a refinement after a simpler query.

### Find contact pages

```text
inurl:contact
```

Example:

```text
"dentist" "Austin" inurl:contact
```

```text
"accounting firm" "Dubai" inurl:contact
```

Possible matching URLs may include:

```text
example.com/contact
example.com/contact-us
example.com/company/contact
```

### Remove URL patterns

Use `-inurl:` to remove URLs containing a pattern.

```text
-inurl:reel
```

```text
-inurl:p
```

### Reduce Instagram posts and reels

```text
site:instagram.com "boutique" "Dubai" ("email" OR "WhatsApp") -inurl:reel -inurl:p
```

This attempts to favor profile pages by removing common reel and post URL patterns.

### Important warning about -inurl:p

`-inurl:p` is broad. It can remove any result with `p` in the matched URL pattern, not only Instagram posts.

Use it mainly with:

```text
site:instagram.com
```

Avoid adding it blindly to general website searches.

Usually unnecessary:

```text
site:.ae "boutique" "Dubai" -inurl:reel -inurl:p
```

Better:

```text
site:.ae "boutique" "Dubai" "contact"
```

Use the Instagram exclusions only when searching Instagram:

```text
site:instagram.com "boutique" "Dubai" -inurl:reel -inurl:p
```

---

## 9. Search by date with after and before

Use `after:` and `before:` when freshness matters.

### Results after a date

```text
after:2025/01/01
```

Example:

```text
"marketing agency" "New York" ("email" OR "WhatsApp") after:2025/01/01
```

### Results before a date

```text
before:2026/01/01
```

Example:

```text
"marketing agency" "New York" before:2026/01/01
```

### Search inside a date range

Combine both operators:

```text
after:2025/01/01 before:2026/01/01
```

Complete example:

```text
"marketing agency" "New York" after:2025/01/01 before:2026/01/01
```

### Year-only searches

You can also use a year:

```text
after:2024
```

```text
before:2026
```

### When dates help

Use date filters for:

- Recently updated directories
- New business announcements
- Current contact pages
- Recent social profile mentions
- Market research limited to a period

### When dates hurt

Many business homepages and contact pages do not display a reliable update date. A date filter can remove an otherwise useful business website.

If results become too limited, remove the dates:

```text
"accounting firm" "Dubai" ("email" OR "WhatsApp")
```

---

## 10. Keep words close with AROUND

`AROUND(n)` asks Google to find two terms within roughly `n` words of each other.

### Syntax

```text
"first term" AROUND(8) "second term"
```

Keep `AROUND` uppercase.

### Business and WhatsApp example

```text
"boutique" AROUND(8) "WhatsApp" "Dubai"
```

This asks for pages where `boutique` and `WhatsApp` appear reasonably close while keeping Dubai relevant.

### Business and email example

```text
"accounting firm" AROUND(10) "email" "London"
```

### Business name and contact example

```text
"Noor Boutique" AROUND(6) "contact"
```

### Choosing the distance

- `AROUND(3)` is strict
- `AROUND(5)` is fairly close
- `AROUND(8)` is a practical starting point
- `AROUND(10)` is broader

### Important limitation

`AROUND(n)` is not currently one of Google's strongly documented customer-facing operators. Its behavior may be inconsistent, and Google may ignore it.

If it produces weak results, simplify the query:

```text
"boutique" "WhatsApp" "Dubai"
```

Do not build your entire search strategy around `AROUND(n)`. Treat it as an optional experiment.

---

## 11. How to combine operators correctly

The safest approach is progressive query building. Add one layer at a time.

### Layer 1: Category and location

```text
"boutique" "Dubai"
```

### Layer 2: Add a contact signal

```text
"boutique" "Dubai" ("email" OR "WhatsApp")
```

### Layer 3: Remove obvious noise

```text
"boutique" "Dubai" ("email" OR "WhatsApp") -jobs -careers -hiring
```

### Layer 4: Choose a source

```text
site:.ae "boutique" "Dubai" ("email" OR "WhatsApp") -jobs -careers -hiring
```

### Layer 5: Prioritize business emails

```text
site:.ae "boutique" "Dubai" ("info@" OR "contact@" OR "sales@" OR "hello@") -jobs -careers -hiring
```

### Layer 6: Add a date only when necessary

```text
site:.ae "boutique" "Dubai" ("info@" OR "contact@" OR "sales@" OR "hello@") after:2025/01/01
```

### Why one layer at a time matters

If the query stops working, you will know which change caused the problem.

If you add six operators at once, you will not know whether the issue came from:

- The category wording
- The location
- The selected platform
- The contact signal
- The exclusions
- The date range
- The URL filter

Simple queries are easier to test, improve and teach.

---

## 12. Copy-ready query templates

Replace `[CATEGORY]`, `[LOCATION]`, `[DOMAIN]` and `[DATE]` before searching.

### Normal category and location

```text
"[CATEGORY]" "[LOCATION]"
```

### Category, location and contact

```text
"[CATEGORY]" "[LOCATION]" "contact"
```

### Remove recruitment pages

```text
"[CATEGORY]" "[LOCATION]" "contact" -jobs -careers -hiring
```

### Remove major social platforms

```text
"[CATEGORY]" "[LOCATION]" "contact" -site:facebook.com -site:instagram.com -site:linkedin.com
```

### Find either email or WhatsApp

```text
"[CATEGORY]" "[LOCATION]" ("email" OR "WhatsApp")
```

### Find role-based business email prefixes

```text
"[CATEGORY]" "[LOCATION]" ("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Business emails without job pages

```text
"[CATEGORY]" "[LOCATION]" ("info@" OR "contact@" OR "sales@" OR "hello@") -jobs -careers -hiring
```

### Search WhatsApp pages

```text
site:wa.me "[CATEGORY]" "[LOCATION]"
```

### Search Instagram profiles

```text
site:instagram.com "[CATEGORY]" "[LOCATION]" ("email" OR "WhatsApp") -inurl:reel -inurl:p
```

### Search LinkedIn companies

```text
site:linkedin.com/company "[CATEGORY]" "[LOCATION]" ("email" OR "contact")
```

### Search Facebook pages

```text
site:facebook.com "[CATEGORY]" "[LOCATION]" ("email" OR "WhatsApp")
```

### Search UAE domains

```text
site:.ae "[CATEGORY]" "[LOCATION]" "contact"
```

### Search UAE domains for business email prefixes

```text
site:.ae "[CATEGORY]" "[LOCATION]" ("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Search contact URLs

```text
"[CATEGORY]" "[LOCATION]" inurl:contact
```

### Search recent mentions

```text
"[CATEGORY]" "[LOCATION]" ("email" OR "WhatsApp") after:[DATE]
```

Example date:

```text
after:2025/01/01
```

### Search a date range

```text
"[CATEGORY]" "[LOCATION]" after:2025/01/01 before:2026/01/01
```

### Keep category and WhatsApp nearby

```text
"[CATEGORY]" AROUND(8) "WhatsApp" "[LOCATION]"
```

### Search a known website

```text
site:[DOMAIN] ("email" OR "WhatsApp")
```

Example:

```text
site:example.com ("email" OR "WhatsApp")
```

### Search a known website for business email prefixes

```text
site:[DOMAIN] ("info@" OR "contact@" OR "sales@" OR "hello@")
```

---

## 13. A realistic search workflow

### Target

Find publicly available contact signals for boutiques in Dubai.

Do not paste every query at the same time. Run each query separately and compare the quality of the results.

### Step 1: Start normally

```text
boutiques in Dubai
```

Purpose:

- Understand how Google describes the market
- Discover common category words
- See whether websites or social profiles dominate
- Identify possible category synonyms

Possible synonyms discovered:

- Fashion boutique
- Clothing store
- Women's fashion
- Modest wear
- Abaya boutique

### Step 2: Require the main concepts

```text
"boutique" "Dubai" "contact"
```

Purpose:

- Keep the business category relevant
- Keep the target location relevant
- Prefer pages mentioning contact information

### Step 3: Remove job pages

```text
"boutique" "Dubai" "contact" -jobs -careers -hiring
```

Purpose:

- Reduce recruitment pages
- Keep customer-facing pages more visible

### Step 4: Reduce social results

```text
"boutique" "Dubai" "contact" -site:facebook.com -site:instagram.com -site:linkedin.com
```

Purpose:

- Find more official websites
- Find directories and contact pages
- Avoid collecting the same business repeatedly from several social platforms

### Step 5: Search UAE business websites

```text
site:.ae "boutique" "Dubai" "contact"
```

Purpose:

- Focus on indexed `.ae` websites
- Find local contact pages and business sites

Remember that some Dubai businesses use `.com`, so this should not be your only query.

### Step 6: Search business email prefixes

```text
site:.ae "boutique" "Dubai" ("info@" OR "contact@" OR "sales@" OR "hello@")
```

Purpose:

- Prefer pages mentioning role-based business emails
- Reduce dependence on personal Gmail addresses

### Step 7: Search WhatsApp pages

```text
site:wa.me "boutique" "Dubai"
```

Purpose:

- Find indexed WhatsApp business pages
- Discover businesses that use WhatsApp as a main contact channel

### Step 8: Search Instagram profiles

```text
site:instagram.com "boutique" "Dubai" ("email" OR "WhatsApp") -inurl:reel -inurl:p
```

Purpose:

- Discover boutiques mainly active on Instagram
- Reduce posts and reels
- Favor profile-style results

### Step 9: Test category synonyms

```text
("fashion boutique" OR "clothing store" OR "modest wear") "Dubai" ("email" OR "WhatsApp")
```

Purpose:

- Find businesses that do not use the exact word `boutique`
- Expand the market without removing location relevance

### Step 10: Test freshness only if needed

```text
"boutique" "Dubai" ("email" OR "WhatsApp") after:2025/01/01
```

Purpose:

- Prefer recently updated or recently indexed pages

If this removes too many business websites, use the same query without the date.

### Step 11: Test proximity only if needed

```text
"boutique" AROUND(8) "WhatsApp" "Dubai"
```

Purpose:

- Test whether keeping the category near the contact word improves relevance

If the results are worse, return to:

```text
"boutique" "WhatsApp" "Dubai"
```

### Step 12: Compare the queries

Do not judge a query by the result count shown at the top of Google. That number is an estimate.

Judge each query by reviewing the first page:

- How many results are actual target businesses?
- How many results are in the correct location?
- How many results show a useful public contact signal?
- How many results are duplicates?
- How many results are outdated or irrelevant?

Keep the simplest query that consistently produces useful businesses.

---

## 14. Troubleshooting poor results

### Problem: Too many job and recruitment pages

Add:

```text
-jobs -careers -hiring
```

### Problem: Too many Facebook, Instagram or LinkedIn results

Add:

```text
-site:facebook.com -site:instagram.com -site:linkedin.com
```

### Problem: You only want Instagram profiles

Use:

```text
site:instagram.com "[CATEGORY]" "[LOCATION]" -inurl:reel -inurl:p
```

### Problem: You want more official websites

Use the master website query:

```text
"[CATEGORY]" "[LOCATION]" "contact" -site:facebook.com -site:instagram.com -site:linkedin.com
```

For UAE businesses, also test:

```text
site:.ae "[CATEGORY]" "[LOCATION]" "contact"
```

### Problem: You want business emails instead of general email mentions

Use:

```text
("info@" OR "contact@" OR "sales@" OR "hello@")
```

Complete example:

```text
"accounting firm" "Dubai" ("info@" OR "contact@" OR "sales@" OR "hello@")
```

### Problem: The query returns almost nothing

Remove filters in this order:

1. Remove `after:` and `before:`
2. Remove `AROUND(n)`
3. Remove `inurl:` or `-inurl:`
4. Remove unnecessary exclusions
5. Remove the source restriction such as `site:.ae`
6. Try category synonyms
7. Return to a normal category and location search

### Problem: The location is being ignored

Put the location in quotes:

```text
"commercial cleaning" "Abu Dhabi"
```

Try the city and country together:

```text
"commercial cleaning" "Abu Dhabi" "UAE"
```

### Problem: site:.ae returns too few businesses

Many UAE businesses use `.com` domains. Remove `site:.ae` and keep the location:

```text
"accounting firm" "Dubai" ("email" OR "WhatsApp")
```

### Problem: AROUND does not improve the results

Remove it:

```text
"boutique" "WhatsApp" "Dubai"
```

`AROUND(n)` is optional and may be ignored.

### Problem: The query is too long to understand

Return to four clear parts:

```text
"[CATEGORY]" "[LOCATION]" [CONTACT SIGNAL] [ONE SOURCE OR EXCLUSION]
```

Example:

```text
"dentist" "Houston" ("email" OR "WhatsApp") -jobs
```

---

## 15. Quick reference

| Goal | Syntax | Example |
| --- | --- | --- |
| Keep a phrase together | `"exact phrase"` | `"commercial cleaning"` |
| Search one domain | `site:domain.com` | `site:wa.me "boutique"` |
| Search UAE domains | `site:.ae` | `site:.ae "accounting firm"` |
| Remove a word | `-word` | `-jobs -careers -hiring` |
| Remove a website | `-site:domain.com` | `-site:facebook.com` |
| Accept alternatives | `(A OR B)` | `("email" OR "WhatsApp")` |
| Find business email prefixes | OR group | `("info@" OR "contact@" OR "sales@" OR "hello@")` |
| Find a URL word | `inurl:word` | `inurl:contact` |
| Remove a URL pattern | `-inurl:word` | `-inurl:reel -inurl:p` |
| Search after a date | `after:YYYY/MM/DD` | `after:2025/01/01` |
| Search before a date | `before:YYYY/MM/DD` | `before:2026/01/01` |
| Keep terms nearby | `AROUND(n)` | `"boutique" AROUND(8) "WhatsApp"` |

## Operators deliberately not included

This handbook does not teach:

- `intitle:`
- `intext:`
- `allintext:`

Their current behavior is too inconsistent for a dependable customer workflow. The queries in this handbook focus on methods that are easier to explain, test and adjust.

## Final rule

Start simple. Change one part at a time. Compare the quality of the businesses, not the estimated number of results.

The best query is not the longest one. It is the shortest query that repeatedly finds relevant businesses in the correct market.

## Responsible use

Use these searches only for legitimate research into publicly available business information.

- Verify that the result belongs to the correct business
- Confirm that the contact information is current
- Follow applicable privacy, consent and marketing rules
- Avoid irrelevant or excessive outreach
- Do not search for passwords, private records, confidential files, exposed systems or sensitive personal information

## Official Google references

- [Refine Google searches](https://support.google.com/websearch/answer/2466433)
- [How to use the site search operator](https://developers.google.com/search/docs/monitor-debug/search-operators/all-search-site)
- [Google Advanced Search](https://www.google.com/advanced_search)

---

Business Contact Extractor by Blaster Pro Tools

