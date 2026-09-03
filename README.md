# hamm-jones-PS
hamm and Jones property Services website


## Live demo (GitHub Pages)
- Site root (redirects to Services): https://sageman2022.github.io/hamm-jones-PS/
- Direct Services page: https://sageman2022.github.io/hamm-jones-PS/services.html#services

I added a Services page based on: https://cairnspade-works.polsia.io/#services and an HTTPS-friendly redirect so the repository root immediately opens the Services section.

What I added to this repository
- `services.html` — Services page copied/mimicked from the provided link.
- `index.html` — Redirects to `./services.html#services` using a meta refresh and a JavaScript fallback (works over HTTPS).

Enable GitHub Pages (one-minute setup)
1. Go to this repository's Settings → Pages.
2. Under "Source" select: Branch = `main`, Folder = `/ (root)` and click Save.
3. After a short time the site will be published at the GitHub Pages URL above and served over HTTPS.

Add a custom domain (HTTPS-friendly)
If you prefer visitors to use your own domain (recommended: a subdomain such as `services.example.com`):

- Create a CNAME DNS record for your chosen subdomain with the value: `sageman2022.github.io`
  - Name: `services` (if you want `services.example.com`)
  - Value / Target: `sageman2022.github.io`
- I can add a `CNAME` file to the repository containing the exact domain (for example: `services.example.com`) — after Pages detects the CNAME GitHub will provision an HTTPS certificate for your custom domain.

Apex/root domains
- If you prefer the apex domain (example.com) instead of a subdomain, create A records pointing to the GitHub Pages IP addresses:
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153
- Then add a `CNAME` file containing the apex domain. GitHub Pages will provision HTTPS once DNS is correct.

Want me to add the CNAME file or further polish the page?
- If you give the exact domain (e.g., `services.example.com`) and confirm I may commit, I will add the `CNAME` file and update the site metadata (OG tags, favicon) as requested.
- I can also add images, pricing, or a contact form to `services.html` — tell me what content or provide image files.
