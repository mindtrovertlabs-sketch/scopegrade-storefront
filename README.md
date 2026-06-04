# Scopegrade Storefront

Static GitHub Pages package for Scopegrade.

## Publish source

Recommended GitHub Pages setting:

- Source: deploy from a branch.
- Branch: main.
- Folder: / root.

GitHub's current docs say GitHub Pages can publish when changes are pushed to a specific branch or via GitHub Actions:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Before publishing

1. Confirm launch_config.json uses real support email and Stripe Payment Links.
2. Run:

`powershell
powershell -ExecutionPolicy Bypass -File .\build_scopegrade_storefront.ps1
powershell -ExecutionPolicy Bypass -File .\prepare_github_pages_package.ps1
powershell -ExecutionPolicy Bypass -File .\verify_github_pages_package.ps1
`

3. User approves final publication.

## Included

- index.html: storefront.
- preview.html: free preview.
- oi-calculator.html: public automation ROI calculator.
- utomation-scoping-review.html: async automation scoping review offer.
- ag-pilot-readiness-review.html: async RAG readiness review offer.
- i-code-review-scorecard-pass.html: async AI code review scorecard offer.
- sync-review-brief.html: redacted brief template for async reviews.
- scopegrade_free_preview.zip: free preview ZIP.
- obots.txt, sitemap.xml, 404.html, .nojekyll.

Paid ZIPs are not included in the public GitHub Pages package. Fulfill paid products through Stripe delivery, support email, or another private delivery path after checkout.

No personal LinkedIn, CV, fake testimonials, fake clients, fake team or guaranteed outcomes.
