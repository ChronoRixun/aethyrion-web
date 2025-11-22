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

### [Nova](tools/nova.html) - Flagship Tool ✨
Your AI Coding Partner - Hundreds of Models, Zero Limits. Free alternative to Cursor, Aider, and GitHub Copilot.
- **Status:** Alpha Testing (Public Release Coming Soon)
- [View Page](tools/nova.html) | [GitHub](https://github.com/AethyrionAI/Nova)

### [Helix](tools/helix.html) - Live ✅
Free alternative to v0.dev and Magic Patterns. Generate React components from text or screenshots.
- **Status:** Live & Available
- [View Page](tools/helix.html) | [Live Site](https://helix.aethyrion.org)

### [Prism](tools/prism.html) - Closed Beta 🔶
ServiceNow development assistant powered by AI.
- **Status:** Closed Beta (Public Release Q2 2026)
- [View Page](tools/prism.html)

---

## 📁 Project Structure

```
aethyrion-web/
├── index.html          # Main landing page (Nova spotlight)
├── tools/              # Individual tool pages
│   ├── nova.html      # Nova - AI coding assistant (FLAGSHIP)
│   ├── helix.html     # Helix - Component generator (LIVE)
│   └── prism.html     # Prism - ServiceNow assistant (BETA)
├── handoffs/          # Design documentation
└── README.md          # This file
```

---

## 🎨 Design

**Main Landing Page:**
- **Nova Spotlight** - Premium hero card featuring flagship tool
- **Pink → Purple → Blue gradient theme** (matches Nova's branding)
- **Animated background** with floating orbs
- **Glassmorphism** cards with backdrop blur
- **Fully responsive** (mobile, tablet, desktop)
- **Pure HTML/CSS** - no dependencies!

**Individual Tool Pages:**
- Each tool has its own **comprehensive page**:
  - Nova: Pink/Purple/Blue gradient (#ec4899 → #8b5cf6 → #3b82f6)
  - Helix: Blue/Cyan (#3b82f6 → #06b6d4)
  - Prism: Purple/Violet (#8b5cf6 → #a855f7)
- Detailed feature breakdowns
- Pricing comparisons vs paid alternatives
- Getting started guides
- Tech stack highlights

---

## 🔧 Recent Updates (November 2025)

### Website Revamp - Nova Flagship Launch
- ✅ Nova added as flagship tool with premium spotlight positioning
- ✅ Removed Observatory, Conduit, Spectra (features absorbed into Nova)
- ✅ Updated to 3-tool ecosystem: Nova, Helix, Prism
- ✅ New pink/purple/blue gradient theme
- ✅ Created comprehensive tools/nova.html page
- ✅ Updated stats: "228+ AI Models", "3 Tools & Growing"
- ✅ Accurate dates: Prism public release Q2 2026
- ⏳ **TODO:** Delete obsolete files: tools/observatory.html, tools/conduit.html, tools/spectra.html

---

## 🔧 Customization

### Update Links
Currently configured:
- Nova GitHub: https://github.com/AethyrionAI/Nova (private during alpha)
- Helix Live Site: https://helix.aethyrion.org
- Discord: https://discord.gg/UZPWT8PxDe
- Reddit: https://www.reddit.com/r/aethyrion

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
<meta property="og:image" content="https://aethyrion.org/og-image.png">
<meta property="og:url" content="https://aethyrion.org">
<meta name="twitter:card" content="summary_large_image">
```

---

## 🚀 Deployment

### Cloudflare Pages (Current Setup)
```bash
# Already deployed to Cloudflare Pages
# Main site: aethyrion.org
# Helix subdomain: helix.aethyrion.org
# Nova subdomain: nova.aethyrion.org (planned)
```

### GitHub Pages
1. Push to GitHub
2. Settings → Pages
3. Source: Deploy from branch (main, /root)

### Vercel / Netlify
```bash
# Install CLI and deploy
vercel  # or netlify deploy --prod
```

---

## 📝 Todo

### Immediate
- [ ] Delete obsolete tool files: observatory.html, conduit.html, spectra.html
- [ ] Test all links and navigation
- [ ] Verify responsive design on mobile

### Nova Subdomain (nova.aethyrion.org)
- [ ] Gather Nova screenshots for showcase
- [ ] Create subdomain landing page (similar to helix.aethyrion.org structure)
- [ ] Feature generated code examples
- [ ] Add download/installation instructions
- [ ] Link to comprehensive documentation
- [ ] Set up Cloudflare Pages deployment
- [ ] Configure custom domain

### Future Enhancements
- [ ] Add favicon (main + per-tool)
- [ ] Add Open Graph images (main + 3 tools)
- [ ] Add analytics (Cloudflare Analytics is free!)
- [ ] Consider newsletter signup for product updates
- [ ] Add testimonials section once Nova is public

---

## 📊 Analytics Insights

**Helix Performance (30 days, zero marketing):**
- 1.2k organic visitors
- Proves strong demand for free developer tools
- Validates Aethyrion's market potential

**Strategy:**
- Leverage Helix's success to drive Nova adoption
- Cross-promote between tools
- Focus on developer communities (Discord, Reddit, GitHub)

---

## 🤝 Contributing

Found a bug or have a suggestion? Open an issue on GitHub!

---

## 📄 License

MIT License - see [LICENSE](LICENSE)

---

**Built with ✨ by Owen**  
*Making professional dev tools free for everyone*

**Current Date:** November 22, 2025 (Q4 2025)
