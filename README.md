# stlwaterdamagehelp

Jekyll site for St. Louis Water Damage Restoration Help.

## Update contact details

Edit `_data/contact.yml` to update company name, phone display, tel link, SMS link, email, hours, locality, and service radius. Header, sticky CTA, sidebars, footer, and schema-oriented content pull from this file.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

## Deployment

GitHub Pages deploys from `.github/workflows/pages.yml`. The `CNAME` file sets the custom domain to `stlwaterdamagehelp.com`. In Cloudflare, point the domain to GitHub Pages using GitHub's current Pages DNS guidance, then keep SSL/TLS in Full mode once GitHub issues the certificate.


## Cloudflare DNS handoff for `stlwaterdamagehelp.com`

GitHub Pages is configured with the custom domain `stlwaterdamagehelp.com`, but Cloudflare DNS must point the domain at GitHub before the custom domain will serve this site. Current DNS may still show Namecheap parking. In Cloudflare DNS, remove parking A/CNAME records and add:

- `A` record for `@` to `185.199.108.153`
- `A` record for `@` to `185.199.109.153`
- `A` record for `@` to `185.199.110.153`
- `A` record for `@` to `185.199.111.153`
- `CNAME` record for `www` to `jules-the-ai.github.io`

Use DNS-only/gray-cloud while GitHub issues the Pages certificate. After GitHub Pages reports the certificate is ready, enable HTTPS enforcement in the repository Pages settings.
