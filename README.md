# Waterfall Farms Website

A simple static website for Waterfall Farms deployed as a Cloudflare Worker.

## Structure
- `public/index.html`: Main page
- `public/css/style.css`: Stylesheet
- `public/js/script.js`: JavaScript (minimal)
- `_worker.js`: Cloudflare Worker script to serve static files
- `wrangler.toml`: Cloudflare Workers configuration
- `package.json`: Dependencies

## Deployment to Cloudflare Workers

1. Install Wrangler: `npm install -g wrangler`
2. Login: `wrangler auth login`
3. Deploy: `wrangler deploy`

The site will be live at your Cloudflare Workers URL.

## Alternative: Cloudflare Pages

If using Pages instead:
1. Go to [Cloudflare Pages](https://pages.cloudflare.com/)
2. Connect your GitHub repository
3. Set build settings:
   - Build command: `npm install && npm run build` (if needed, but static)
   - Build output directory: `public`
4. Deploy