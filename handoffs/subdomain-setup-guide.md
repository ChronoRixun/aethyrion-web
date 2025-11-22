# Aethyrion Subdomain Setup Guide
**Setting up tool-specific subdomains using Cloudflare Pages**

## Why This Approach?

**Consistency**: Keep all your web properties in the Cloudflare ecosystem (same as aethyrion.org)
**Free**: Unlimited Cloudflare Pages projects on free tier
**Simple**: Same workflow you already know from the main site
**Professional**: Each tool gets its own polished web presence

## The Structure

```
aethyrion.org          → Main landing page (ecosystem overview)
helix.aethyrion.org    → Helix tool page (download, docs, demos)
prism.aethyrion.org    → Prism tool page (when ready)
observatory.aethyrion.org → Observatory (future)
```

---

## Step-by-Step: Setting Up Your First Subdomain (Helix)

### Phase 1: Prepare the Helix Web Content

1. **Create a new directory** for Helix's web presence
   - Could be a new repo: `helix-web` or `helix-landing`
   - Or a folder in your existing Helix repo (if you want docs/landing together)

2. **Build a simple landing page** for Helix
   - **Recommended structure**:
     ```
     helix-web/
     ├── index.html
     ├── styles.css (optional)
     └── assets/ (screenshots, icons, etc.)
     ```

3. **What to include** (MVP):
   - Brief description of Helix
   - Download button/link to the GitHub release
   - Quick feature list
   - Link back to main aethyrion.org
   - Screenshot or demo (when you have them)

**Design Tip**: Keep the same visual language as aethyrion.org (dark theme, blue-purple gradients, glassmorphism). This creates brand cohesion.

---

### Phase 2: Deploy to Cloudflare Pages

1. **Push your Helix web content to GitHub**
   - Make sure it's in a public repo
   - Main file should be `index.html` in the root (or specify build output)

2. **Go to Cloudflare Dashboard**
   - Navigate to: `Workers & Pages` → `Create application` → `Pages` → `Connect to Git`

3. **Connect the Repository**
   - Authorize GitHub if needed
   - Select your `helix-web` repo (or whatever you named it)

4. **Configure Build Settings**
   - **Framework preset**: None (if just HTML/CSS)
   - **Build command**: Leave empty (unless you're using a build tool)
   - **Build output directory**: `/` (or wherever your index.html is)

5. **Deploy**
   - Click `Save and Deploy`
   - Cloudflare will give you a default URL like: `helix-web.pages.dev`
   - Test this URL to make sure everything works

---

### Phase 3: Set Up the Custom Subdomain

1. **In Cloudflare Pages Project Settings**
   - Go to your newly deployed Helix project
   - Click `Custom domains` tab
   - Click `Set up a custom domain`

2. **Add Your Subdomain**
   - Enter: `helix.aethyrion.org`
   - Cloudflare will automatically:
     - Create the DNS record for you
     - Set up SSL certificate
     - Configure routing

3. **Wait for DNS Propagation**
   - Usually takes 1-5 minutes
   - Status will show "Active" when ready

4. **Test It**
   - Visit `https://helix.aethyrion.org`
   - Should show your Helix landing page
   - SSL should work automatically (check for the padlock 🔒)

---

## Best Practices & Recommendations

### Repository Organization

**Option A: Separate Web Repos** (Recommended for you)
```
aethyrion-web/         → Main landing page
helix-web/             → Helix landing/docs
prism-web/             → Prism landing/docs
observatory-web/       → Observatory landing/docs
```
**Pros**: Clean separation, easier to manage permissions later
**Cons**: More repos to track

**Option B: Monorepo**
```
aethyrion-web/
├── main/              → aethyrion.org
├── helix/             → helix.aethyrion.org
├── prism/             → prism.aethyrion.org
└── shared/            → Shared components/styles
```
**Pros**: Everything in one place, shared assets
**Cons**: More complex deployment setup

### Content Strategy for Tool Pages

Each subdomain should answer:
1. **What is this tool?** (1-2 sentence pitch)
2. **Why would I use it?** (problem it solves)
3. **How do I get it?** (download button, clear CTA)
4. **Where can I learn more?** (docs, GitHub, Discord)

**Keep it simple**: Don't overcomplicate. A single scrolling page is often perfect.

### Linking Strategy

- **Main site** (aethyrion.org): Shows all tools, links to subdomains
- **Each tool subdomain**: Has a "Back to Aethyrion" link
- **Cross-promotion**: "Using Helix? Check out Prism"

### Visual Consistency

Since you have a design system established:
- **Reuse CSS** across properties (consider a shared stylesheet)
- **Same color palette**: #0f172a, #1e293b, #3b82f6, #8b5cf6
- **Same glassmorphism effects**
- **Same typography choices**

This makes the entire ecosystem feel cohesive and professional.

---

## Rinse and Repeat for Other Tools

Once you have Helix set up, the process for Prism/Observatory/etc is identical:

1. Create tool landing page content
2. Push to GitHub repo
3. Deploy to Cloudflare Pages
4. Add custom domain: `toolname.aethyrion.org`
5. Test and launch

**Each additional subdomain takes ~10-15 minutes once you have the content ready.**

---

## Common Issues & Solutions

### Issue: DNS Not Propagating
**Solution**: Wait 5-10 minutes. Check status in Cloudflare DNS panel.

### Issue: SSL Certificate Pending
**Solution**: Cloudflare auto-provisions this. Usually takes 1-2 minutes.

### Issue: 404 on Subdomain
**Solution**: Check that `index.html` is in the correct directory as specified in build settings.

### Issue: Old Content Showing
**Solution**: Cloudflare Pages caches aggressively. Either:
- Wait a few minutes for auto-refresh
- Use "Retry deployment" in Pages dashboard

---

## Future Considerations

### Analytics
Cloudflare has built-in Web Analytics (free). Consider adding this to track:
- Which tools get the most traffic
- Where users come from
- What to prioritize

### Documentation Hosting
For more complex docs, consider:
- **docs.aethyrion.org** → Centralized docs for all tools
- Or tool-specific: **helix.aethyrion.org/docs**

### API Endpoints (Future)
If any tools need backend APIs:
- Cloudflare Workers (free tier is generous)
- Keep them on subdomains: `api.helix.aethyrion.org`

---

## Quick Reference Commands

**Check DNS propagation**:
```bash
nslookup helix.aethyrion.org
```

**Test SSL certificate**:
```bash
curl -I https://helix.aethyrion.org
```

**Force HTTPS redirect** (Cloudflare does this automatically, but verify in SSL/TLS settings):
- Cloudflare Dashboard → SSL/TLS → Edge Certificates → Always Use HTTPS = ON

---

## Questions to Consider

1. **Do you want a unified documentation site**, or docs per tool?
2. **Should each tool page include a demo/playground?** (Could be a helix.aethyrion.org/demo page)
3. **Community links**: Should each subdomain link to Discord/Reddit, or just the main site?
4. **Download hosting**: GitHub Releases vs Cloudflare R2 (both free, GitHub is simpler)

---

**You're ready to go!** Start with Helix, and you'll have the pattern down for the rest of the ecosystem.