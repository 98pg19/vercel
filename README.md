# Fund Now

A simple donation page with Vercel Web Analytics integration.

## Features

- Clean, responsive landing page
- PayPal donation integration
- Vercel Web Analytics for tracking page views and visitor metrics

## Analytics Setup

This project uses Vercel Web Analytics to track visitor data. The analytics are integrated via the static HTML method as documented in the [Vercel Analytics Quickstart](https://vercel.com/docs/analytics/quickstart).

### How it works

The analytics script is loaded in `public/index.html`:

```html
<script>
  window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>
```

### Enabling Analytics

1. Go to your Vercel project dashboard
2. Navigate to the Analytics section
3. Click "Enable" to activate Web Analytics
4. Deploy the project
5. Analytics data will appear in your dashboard after visitors access your site

## Deployment

Deploy to Vercel:

```bash
vercel deploy
```

Or connect your Git repository for automatic deployments on push.

## Development

This is a static site with no build process required. Simply open `public/index.html` in a browser for local development.
