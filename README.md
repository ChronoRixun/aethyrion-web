# Aethyrion Ecosystem Website

**Free Developer Tools for Everyone**

Official landing page for the Aethyrion ecosystem of free, open-source developer tools.

---

## 🚀 Quick Start

1. Open `index.html` in a browser, or
2. Deploy to any static hosting (Vercel, Netlify, GitHub Pages, Cloudflare Pages)

That's it! No build step required.

---

## 🌟 Featured Tools

### [Helix](tools/helix.html) - Live ✅
Free alternative to v0.dev and Magic Patterns. Generate React components from text or screenshots.
- [View Page](tools/helix.html) | [GitHub](#)

### [Prism](tools/prism.html) - Beta 🔶
ServiceNow development assistant powered by AI.
- [View Page](tools/prism.html) | [GitHub](#)

### [Observatory](tools/observatory.html) - In Development 🚧
Self-hosted observability platform (Datadog/New Relic alternative)
- [View Page](tools/observatory.html) | [GitHub](#)

### [Conduit](tools/conduit.html) - Coming Soon 📦
AI-powered API testing & documentation (Postman alternative)
- [View Page](tools/conduit.html) | [GitHub](#)

### [Spectra](tools/spectra.html) - In Development 🌈
AI-powered code review agent (CodeRabbit/Codacy alternative)
- [View Page](tools/spectra.html) | [GitHub](#)

---

## 📁 Project Structure

```
aethyrion-web/
├── index.html          # Main landing page
├── tools/              # Individual tool pages
│   ├── helix.html     # Helix - AI component generator (LIVE)
│   ├── prism.html     # Prism - ServiceNow assistant (BETA)
│   ├── observatory.html # Observatory - Self-hosted observability (DEV)
│   ├── conduit.html   # Conduit - API testing (COMING SOON)
│   └── spectra.html   # Spectra - Code review (DEV)
├── handoffs/          # Design documentation
│   ├── LANDING_PAGE_HANDOFF.md
│   └── WEBSITE_UPDATE_HANDOFF.md
└── README.md          # This file
```

---

## 🎨 Design

**Main Landing Page:**
- **Dark Theme** with blue-purple gradients
- **Animated background** with floating orbs
- **Glassmorphism** cards with backdrop blur
- **Fully responsive** (mobile, tablet, desktop)
- **Pure HTML/CSS** - no dependencies!

**Individual Tool Pages:**
- Each tool has its own **color theme**:
  - Helix: Blue/Cyan (#3b82f6 → #06b6d4)
  - Prism: Purple/Violet (#8b5cf6 → #a855f7)
  - Observatory: Orange/Amber (#fb923c → #f59e0b)
  - Conduit: Cyan/Teal (#06b6d4 → #14b8a6)
  - Spectra: Rainbow gradient (#ec4899 → #8b5cf6 → #3b82f6)
- Comprehensive feature breakdowns
- Pricing comparisons vs paid alternatives
- Getting started guides
- Tech stack highlights

---

## 🔧 Customization

### Update Links
Search for `href="#"` and `href="https://github.com"` in `index.html` and replace with:
- Your GitHub org/repo URLs
- Helix deployment URL
- Prism deployment URL (when ready)
- Discord invite link
- Documentation URL

### Add Analytics
Add your tracking code before `</body>`:
```html
<!-- Google Analytics, Plausible, Fathom, etc. -->
<script>/* Your analytics code */</script>
```

### Add Meta Tags
Add these in `<head>` for better social sharing:
```html
<meta property="og:title" content="Aethyrion - Free Developer Tools">
<meta property="og:description" content="Professional-grade dev tools that cost $20-100/month? Now free forever.">
<meta property="og:image" content="https://aethyrion.com/og-image.png">
<meta property="og:url" content="https://aethyrion.com">
<meta name="twitter:card" content="summary_large_image">
```

---

## 🚀 Deployment

### Vercel
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Netlify
```bash
# Install Netlify CLI
npm i -g netlify-cli

# Deploy
netlify deploy --prod
```

### GitHub Pages
1. Push to GitHub
2. Settings → Pages
3. Source: Deploy from branch (main, /root)

### Cloudflare Pages
1. Push to GitHub
2. Connect repo in Cloudflare Pages
3. Build: None (static HTML)
4. Output: ./

---

## 📝 Todo

- [ ] Update GitHub links (all 5 tools)
- [ ] Add Helix live URL
- [ ] Add Prism download URL
- [ ] Add Discord invite link
- [ ] Add favicon (main + per-tool)
- [ ] Add Open Graph images (main + 5 tools)
- [ ] Add analytics (Google Analytics, Plausible, etc.)
- [ ] Add screenshots/demos to tool pages
- [ ] Consider subdomain setup (helix.aethyrion.org, etc.)
- [ ] Consider newsletter signup

---

## 🤝 Contributing

Found a bug or have a suggestion? Open an issue!

---

## 📄 License

MIT License - see [LICENSE](LICENSE)

---

**Built with 🌀 by Owen**  
*Making professional dev tools free for everyone*
