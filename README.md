# stlwaterdamagehelp

Jekyll lead-generation site for St. Louis water damage restoration searches.

## Swap contact details

Edit `_data/contact.yml` to update company name, phone display, tel link, SMS link, email, hours, locality, and service radius. Header, sticky CTA, sidebars, footer, and schema-oriented content pull from this file.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

## Deployment

GitHub Pages deploys from `.github/workflows/pages.yml`. The `CNAME` file sets the custom domain to `stlwaterdamagehelp.com`. In Cloudflare, point the domain to GitHub Pages using GitHub's current Pages DNS guidance, then keep SSL/TLS in Full mode once GitHub issues the certificate.
