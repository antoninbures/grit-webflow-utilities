# Grit Webflow Utilities

Extracted Webflow utility classes for layout helpers missing from the optimized stylesheet.

Use the minified file in Webflow:

```html
<link rel="stylesheet" href="https://raw.githubusercontent.com/antoninbures/grit-webflow-utilities/main/webflow-utilities.min.css">
```

## CRM scripts

Page-specific Customer Insights snippets are stored in `crm-scripts/`.

- `crm-scripts/invoice-flow-cz-contact-form.html` - fixed Form Capture script for `https://www.grit.eu/invoice-flow`.
- `crm-scripts/kontakt-cz-contact-form.html` - fixed Form Capture script for `https://www.grit.eu/kontakt`.
- `crm-scripts/ebook-form-cz.html` - fixed Form Capture script for e-book detail pages.
- `crm-scripts/lokia-wms-cz-contact-form.html` - fixed Form Capture script for `https://www.grit.eu/skladovy-system-lokia-wms`.
- `crm-scripts/orion-edi-cz-contact-form.html` - fixed Form Capture script for `https://www.grit.eu/elektronicka-vymena-dat-orion-edi`.
- `crm-scripts/e-fakturacia-localized-contact-form.html` - localized e-invoicing form script; CRM capture on SK, redirect only on CZ and EN.
- `crm-scripts/webflow-localized-success-redirect.html` - CRM-independent localized redirect after a successful Webflow form submission.
- `crm-scripts/event-localized-success-redirect.html` - localized registration thank-you redirect for event forms.
