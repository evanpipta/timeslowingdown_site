# timeslowingdown

Static website for the electronic music artist **timeslowingdown**. Built with [Astro](https://astro.build) and deployed to GitHub Pages.

## Local Development

```bash
npm install
npm run dev
```

The dev server starts at `http://localhost:4321`.

## Build

```bash
npm run build
```

Static output is generated in the `dist/` directory.

## Preview Production Build

```bash
npm run preview
```

## Deployment

The site auto-deploys to GitHub Pages on every push to `main` via the workflow in `.github/workflows/deploy.yml`.

### Custom Domain

1. Add your domain to `public/CNAME` (e.g. `timeslowingdown.com`).
2. In GitHub repo settings, go to **Settings > Pages** and set the custom domain.
3. Configure your DNS provider to point to GitHub Pages:
   - For an apex domain: add `A` records pointing to GitHub's IPs (`185.199.108-111.153`).
   - For a subdomain: add a `CNAME` record pointing to `<username>.github.io`.
4. Enable "Enforce HTTPS" in Pages settings once DNS propagates.
