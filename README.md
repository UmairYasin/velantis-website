# Velantis investor site

Static investor-facing site for Velantis (agentic AI-native healthcare integration engine). Built with
[Astro](https://astro.build) + Tailwind CSS — no backend, no server costs.

## Pages

- `/` — home
- `/product` — agentic pipeline, 8 capabilities, connectors
- `/technology` — architecture, HL7 standards, AI approach
- `/security` — compliance posture, security architecture
- `/roadmap` — phased rollout, traction
- `/team` — founder (edit `src/pages/team.astro` to add your bio/photo)
- `/contact` — mailto CTA for investor inquiries

## Local development

```sh
npm install
npm run dev      # http://localhost:4321
npm run build    # outputs to ./dist
npm run preview  # serve the production build locally
```

## Deploying (free tier, ~$10/year total — just the domain)

1. Push this repo to GitHub.
2. Create a [Cloudflare Pages](https://pages.cloudflare.com/) project, connect the GitHub repo.
   - Build command: `npm run build`
   - Output directory: `dist`
3. Cloudflare Pages gives you a free `*.pages.dev` URL immediately, with free SSL and unlimited bandwidth.
4. Buy `velantishealth.com` (or your chosen domain) via [Cloudflare Registrar](https://www.cloudflare.com/products/registrar/)
   (sold at wholesale price, ~$10/yr, no markup) and attach it to the Pages project under
   **Custom domains**.
5. (Optional) Set up [Cloudflare Email Routing](https://developers.cloudflare.com/email-routing/) — free —
   to forward `contact@velantishealth.com` to your real inbox.

Every push to `main` redeploys automatically.
