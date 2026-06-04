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
- i_automation_roi_kit.zip: paid product file.
- ag_eval_kit.zip: paid product file.
- i_code_review_pack.zip: paid product file.
- obots.txt, sitemap.xml, 404.html, .nojekyll.

No personal LinkedIn, CV, fake testimonials, fake clients, fake team or guaranteed outcomes.
