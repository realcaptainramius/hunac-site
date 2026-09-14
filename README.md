# hunac-site

The root hunacenterprises.com marketing site — home, apps, about, and a
contact/quote page. Plain static HTML, no build step.

Consolidates what used to be four separate forms (Home, /contact, /about,
and the fake-checkout Store) into one contact/quote page. The Store's real
paid products (photo shoots) were dropped along with the rest of Squarespace
Commerce, per the decision to not build a payment backend for this.

Contact form currently opens a pre-filled email via `mailto:` — no backend
yet. Once email routing/forwarding is set up for the domain, this should be
swapped for a real form POST to a Worker endpoint instead.

Deployed via Cloudflare Workers, connected to this GitHub repo.

## Local preview

```bash
npx serve .
```
