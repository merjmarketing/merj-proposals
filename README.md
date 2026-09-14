# merj-proposals

Client-facing pages for Merj Marketing, published with GitHub Pages at https://proposals.merj.marketing

- `discovery/` — Discovery Call Prep Questionnaire
- `<client-slug>/` — one folder per proposal (`index.html` rendered from the proposal template, plus `walkthrough.mp3`)
- `CNAME` — custom domain for GitHub Pages
- `index.html` — root redirects to merj.marketing (proposal URLs are unlisted)

## Deploy, once
1. Push this folder to a new repo `merj-proposals` on GitHub (main branch).
2. Settings → Pages → Source: Deploy from a branch, `main` / root. Custom domain: `proposals.merj.marketing`. Enforce HTTPS.
3. GoDaddy DNS: CNAME record, host `proposals`, value `<github-org>.github.io`.
4. Web3Forms: create an access key with the Basecamp Sales forward address as the notification email. Paste it into `discovery/index.html` (CONFIG.forms.accessKey) and into each proposal's `forms.accessKey`.

## Add a proposal
1. Render the proposal from the template (see the Sales & CRM Pipeline SOP, stage 5).
2. Save as `<client-slug>/index.html`, add `walkthrough.mp3` next to it.
3. Commit and push. Live in about a minute at `https://proposals.merj.marketing/<client-slug>/`.
