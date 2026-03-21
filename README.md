# Canadian Take-Home Pay Calculator

This repository contains a static SimpleKit calculator for estimating take-home pay in Canada.

The tool is designed as a guided salary planning experience that:

- starts with tax year, province or territory, and monthly gross salary
- estimates federal tax, provincial or territorial tax, CPP or QPP, and EI
- shows annual and monthly take-home pay
- estimates when CPP or QPP and EI may be fully paid for the year
- compares the same salary across all provinces and territories

## File Structure

```text
/
  index.html
  calculator-spec.yaml
  assets/
    css/
      styles.css
    js/
      app.js
      simplekit-tool-links.js
```

## Main Files

### `index.html`

Contains:

- SEO metadata
- JSON-LD
- guided calculator layout
- educational content
- FAQ
- related tools section
- shared SimpleKit shell mount points

### `assets/js/app.js`

Contains:

- tax-year configuration data
- province and territory tax logic
- CPP, QPP, and EI estimation logic
- paid-up month estimates
- province comparison rendering
- URL state syncing and share-link support

### `assets/css/styles.css`

Contains:

- local calculator styling
- hero and panel layout
- guided form styling
- results and comparison table styling
- responsive behavior for mobile and desktop

## Shared SimpleKit Connection

This tool keeps the shared SimpleKit shell integration intact:

- `window.SimpleKitPage`
- `data-simplekit-header`
- `data-simplekit-support`
- `data-simplekit-footer`
- `https://core.simplekit.app/core.css`
- `https://core.simplekit.app/core.js`

## Notes

- The calculator is static-site friendly and does not require a build step.
- It is intended as a planning estimate, not payroll or tax advice.
- Future annual updates should focus on the tax-year data tables in `assets/js/app.js`.
