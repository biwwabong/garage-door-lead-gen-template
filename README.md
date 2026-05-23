# garage-door-lead-gen-template

Static lead-gen site with a hybrid asset layout and `npm run build` pipeline.

## Structure

```
assets/images/
  shared/              # Site-wide assets (e.g. dimensions.json)
  components/          # Component imagery (why-choose, etc.)
  sections/            # Reusable section imagery
    hero/
    services/
    callouts/
    engineer-repairs/
    recent-fittings/
    reviews/
  areas/
    werrington/        # Area-specific photos

components/
  partials/            # Shared: header, footer, config, hero form, CTA
  sections/            # Shared section blocks (e.g. why-choose-us)
  pages/               # Page-specific components
    home/
    area-template/
    services/
    contact/
    quote/
    faq/
  styles/
    main.css           # Built stylesheet (linked from pages)
    source.css         # Source copy for editing
  scripts/             # Reserved for component JS

pages/                 # HTML templates (source of truth)
areas.json             # Area page data
scripts/               # build.js, generate-areas.js, replace-variables.js
```

## Build

```bash
npm run build
```

Assembles `pages/*.html` (except `area-template.html`) and generates area pages (e.g. `werrington.html`) into the project root. Edit templates under `pages/` and `components/`, not generated root HTML.
# garage-door-lead-gen-template
