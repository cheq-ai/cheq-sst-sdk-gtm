# CHEQ Manage - Server-Side Tagging (SST) - Web SDK template for Google Tag Manager

This Google Tag Manager (GTM) custom tag template loads and configures the CHEQ Server-Side Tagging (SST) Web SDK. Moving tag execution server-side delivers faster website performance, more complete data collection, better security, and data leakage prevention.

## Installation

**From the Community Template Gallery (recommended):**

1. In your GTM web container, go to **Templates > Tag Templates > Search Gallery**.
2. Search for **CHEQ** and add the [*CHEQ Manage - Server-Side Tagging - Web SDK*](https://tagmanager.google.com/gallery/#/owners/cheq-ai/templates/cheq-sst-sdk-gtm) template.
3. Create a new tag from the template and configure it (see below).

We recommend firing the tag on an **All Pages** trigger so SST integrations work across your entire site.

**Manual import:** download `template.tpl` from this repository, then in GTM go to **Templates > Tag Templates > New**, open the overflow menu, and choose **Import**.

> **Note:** This tag only makes the SST Web SDK available on your pages. To track events, configure tags using the [*CHEQ Manage - Server-Side Tagging - Event*](https://tagmanager.google.com/gallery/#/owners/cheq-ai/templates/cheq-sst-event-gtm) template for each event you want to track (e.g., page view, add to cart).

## Configuration

| Field | Description |
|---|---|
| **Account Name** | Your CHEQ account name (required). |
| **Domain** | Your first-party CHEQ SST domain (recommended), or `t.nc0.co` as a third-party domain (required). |
| **Custom Data** | Key/value pairs added to the SST event that may not be in your data layer; exposed as the `customData` variable within the SST browser. |
| **Storage** | Cookies, localStorage, and sessionStorage entries to set automatically in the SST instance. |
| **Integrations** | One-click support for Bing UET, CHEQ Enforce (Ensighten Privacy) consent, and Google Ads & Floodlight. Identifiers are passed and set automatically so those tags work without customization. |
| **Options** | Event batching and dispatch timing (every # milliseconds, or only when the page is hidden or unloaded), publish path, custom request parameters, and data layer name. |
| **Virtual Browser Overrides** | Override specific virtual browser values (e.g. page URL, referrer, language, Global Privacy Control) sent with the SST request. |
| **High Entropy User-Agent Hints** | The High Entropy User-Agent Hints to collect (e.g. architecture, model, platform version). The values are added to the virtual browser data sent with the SST request; none are requested unless selected. |

## Documentation & support

- [Implementation with Google Tag Manager](https://help.ensighten.com/hc/en-us/articles/36258326811665-Implementation-with-Google-Tag-Manager)
- [CHEQ Manage](https://cheq.ai/manage/)

For help, contact CHEQ support through the [help center](https://help.ensighten.com/).

## License

Licensed under the [Apache License 2.0](LICENSE).
