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

### [Helix](https://github.com/yourusername/helix) - Live ✅
Free alternative to v0.dev and Magic Patterns. Generate React components from text or screenshots.

### [Prism](https://github.com/yourusername/prism) - Beta 🔶
ServiceNow development assistant powered by AI.

### Observatory - Coming Soon 📊
Self-hosted observability platform (Datadog/New Relic alternative)

### Conduit - Coming Soon 🔌
AI-powered API testing & documentation (Postman alternative)

---

## 📁 Project Structure

```
aethyrion-web/
├── index.html          # Main landing page (single file!)
├── handoffs/           # Design documentation
│   └── LANDING_PAGE_HANDOFF.md
└── README.md           # This file
```

---

## 🎨 Design

- **Dark Theme** with blue-purple gradients
- **Animated background** with floating orbs
- **Glassmorphism** cards with backdrop blur
- **Fully responsive** (mobile, tablet, desktop)
- **Pure HTML/CSS** - no dependencies!

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

- [ ] Update GitHub links
- [ ] Add Helix live URL
- [ ] Add Prism URL when ready
- [ ] Add Discord invite
- [ ] Add favicon
- [ ] Add Open Graph image
- [ ] Add analytics
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
