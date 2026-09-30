# Grit Webflow Utilities

Extracted Webflow utility classes for layout helpers missing from the optimized stylesheet.

Use the minified file in Webflow:

```html
<link rel="stylesheet" href="https://raw.githubusercontent.com/antoninbures/grit-webflow-utilities/main/webflow-utilities.min.css">
```

## CRM scripts

Page-specific Customer Insights snippets are stored in `crm-scripts/`.

- `crm-scripts/invoice-flow-cz-contact-form.html` - Form Capture script for `https://www.grit.eu/invoice-flow` and its SK/EN versions. Webflow submits first, then CRM, then redirect only after the CRM confirmed.
- `crm-scripts/kontakt-cz-contact-form.html` - Form Capture script for the Kontakt form (`https://www.grit.eu/kontakt` and the homepage, CZ/SK/EN). Webflow submits first, then CRM, then redirect only after the CRM confirmed.
- `crm-scripts/ebook-form-cz.html` - fixed Form Capture script for e-book detail pages.
- `crm-scripts/lokia-wms-cz-contact-form.html` - Form Capture script for `https://www.grit.eu/skladovy-system-lokia-wms` and its SK/EN versions. Webflow submits first, then CRM, then redirect only after the CRM confirmed. Keeps the MSCI `FormSubmit` tracking event.
- `crm-scripts/orion-edi-cz-contact-form.html` - Form Capture script for `https://www.grit.eu/elektronicka-vymena-dat-orion-edi` and its SK/EN versions. Webflow submits first, then CRM, then redirect only after the CRM confirmed.
- `crm-scripts/e-fakturacia-sk-contact-form.html` - SK e-invoicing form (`/sk/riesenie/e-fakturacia`), includes the package select `variant` -> `grit_doplnenivyberubalicku`. Webflow first, then CRM, then redirect.
- `crm-scripts/e-fakturace-cz-en-contact-form.html` - CZ/EN e-invoicing (`/reseni/e-fakturace`, `/en/solution/e-invoicing`). No CRM form exists yet for these languages (`FormId: null`), so the script only redirects after Webflow succeeded. Fill in the FormIds once available.
- `crm-scripts/{zrychleni-obchodniho-toku,integrace-dodavatelu,automatizace-dokumentu,sscc-kody}-localized-contact-form.html` - `/reseni/*` forms (`#wf-form-Reseni_Form`), CZ/SK/EN in one script. The hidden `source` field carries the page name, so it is listed as an alias of option 4.
- `crm-scripts/odvetvi-{retail,e-commerce,farmacie}-contact-form.html` - `/odvetvi/*` industry forms (`#wf-form-Odvetvi_Form`), FormIds from the CRM mail of 15 Sep 2026. The textarea is `Message` (capital M); `source` holds the industry name and is aliased to option 4.
- `crm-scripts/webflow-localized-success-redirect.html` - CRM-independent localized redirect after a successful Webflow form submission.
- `crm-scripts/event-localized-success-redirect.html` - localized registration thank-you redirect for event forms.
