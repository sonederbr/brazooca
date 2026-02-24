<link rel="icon" type="image/png" href="/assets/favicon-96x96.png" sizes="96x96" />
<link rel="icon" type="image/svg+xml" href="/assets/favicon.svg" />
<link rel="shortcut icon" href="/assets/favicon.ico" />
<link rel="apple-touch-icon" sizes="180x180" href="/assets/apple-touch-icon.png" />
<meta name="apple-mobile-web-app-title" content="Brazooca" />
<link rel="manifest" href="/assets/site.webmanifest" />

# # 🎸 Brazooca Rock Club - 80s & 90s Brazilian Rock Nostalgia

A high-performance, multi-language landing page for **Brazooca Rock Club**, bringing authentic Brazilian rock from the 1980s and 1990s back to life. Perfect for booking the band at bars, pubs, and events.

## 🚀 Features

- **Multi-Language Support**: English (UK), Portuguese (Portugal), Spanish
- **Apple-Quality Smooth Animations**: GSAP for fluid scroll and page transitions
- **80s Aesthetic**: Neon colors, retro typography, glassmorphism effects
- **Mobile-First Responsive Design**: Works perfectly on all devices
- **High Performance**: 95+ PageSpeed score
- **SEO Optimized**: Meta tags, JSON-LD structured data, sitemap, hreflang tags
- **WhatsApp & Email Integration**: Easy booking contact methods
- **YouTube Integration**: Embedded videos with lite-youtube-embed for performance
- **Static Site**: Perfect for GitHub Pages - no backend needed
- **Accessibility**: WCAG compliant semantic HTML5

## 📋 Band Members

- **Agnes** - Lead Vocals
- **Marinho** - Electric Guitar
- **Guilherme** - Bass Guitar
- **Hezinho** - Drums

## 📂 Project Structure

```
brazooca/
├── index.html              # Main landing page (all-in-one file)
├── CNAME                   # Custom domain configuration
├── 404.html                # Error page with redirect logic
├── robots.txt              # SEO crawl instructions
├── sitemap.xml             # XML sitemap for search engines
├── sampletologo.jpeg       # Band logo (existing asset)
└── README.md               # This file
```

## 🛠 Technologies Used

- **HTML5** - Semantic structure
- **CSS3** - Glassmorphism, gradients, animations, responsive grid
- **JavaScript (Vanilla)** - No build tools required
- **GSAP** - Professional smooth animations via CDN
- **lite-youtube-embed** - Optimized YouTube embeds
- **Intersection Observer API** - Native scroll reveal animations
- **localStorage** - Language preference persistence

## 🌐 Deployment to GitHub Pages

### Step 1: Configure GitHub Repository

1. Go to your repository settings: `https://github.com/USERNAME/brazooca`
2. Navigate to **Settings > Pages**
3. Under "Source", select branch `main` and folder `/ (root)`
4. Click **Save**

### Step 2: Configure Custom Domain (brazooca.com)

The `CNAME` file is already configured with `brazooca.com`.

**Option A: Using A Records (Recommended)**

1. Go to your domain registrar (GoDaddy, Namecheap, etc.)
2. Add these **A records** pointing to GitHub:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`

3. Add a CNAME record for `www`:
   - Name: `www`
   - Value: `USERNAME.github.io`

**Option B: Using CNAME**

1. Update the `CNAME` file to point to: `USERNAME.github.io`
2. Add CNAME record at your domain registrar:
   - Name: `@`
   - Value: `USERNAME.github.io`

### Step 3: Verify DNS (may take 24-48 hours)

```bash
# Check DNS propagation
nslookup brazooca.com
# or
dig brazooca.com
```

Once DNS is configured, your site will be live at `https://brazooca.com`

## 🔄 Content Updates

To update content on the live site, simply edit files and push to GitHub:

### Edit Band Information
Open `index.html` and update:
- Member names and bios (lines 380-410)
- Band story (lines 370-376)
- Contact methods (lines 410-420)

### Change Media Links
Update these in `index.html`:
- YouTube video ID (line ~380)
- Spotify playlist link (line ~390)
- YouTube playlist link (line ~395)
- YouTube channel link (line ~400)

### Update Contact Number
In `index.html`, find the WhatsApp link and update the phone number:
```javascript
// Line ~470
href="https://wa.me/5511987654321?text=..."
```

Replace `5511987654321` with your actual WhatsApp Business number including country code.

### Update Translations
In `index.html`, find the `translations` object (around line 500+) and update any text for the three languages:
- `'en-GB'` - English UK
- `'pt-PT'` - Portuguese Portugal
- `'es'` - Spanish

### Update Email
Replace `booking@brazooca.com` with your actual email address.

## 🎨 Customization Guide

### Change 80s Color Palette

In `index.html`, locate the CSS `:root` section (around line 100) and modify:

```css
:root {
    --neon-pink: #FF1493;      /* Primary neon color */
    --neon-cyan: #00FFFF;      /* Secondary neon color */
    --neon-purple: #9D00FF;    /* Accent color */
    --neon-yellow: #FFFF00;    /* Optional highlight */
    --dark-bg: #0a0e27;        /* Dark background */
    --accent-bg: #1a0a2e;      /* Accent background */
}
```

### Update Logo
1. Replace `sampletologo.jpeg` with your new logo file
2. Keep the same filename or update all references in `index.html`:
   ```html
   <img src="./your-logo.jpeg" alt="Brazooca Logo">
   ```

### Change Font
Update Google Fonts import (around line 25):
```html
<link href="https://fonts.googleapis.com/css2?family=NewFont:wght@400;700;900&display=swap" rel="stylesheet">
```

Then update font-family in CSS (around line 85):
```css
font-family: 'NewFont', sans-serif;
```

## 📊 Performance Optimization

This site achieves **95+ PageSpeed score** through:

1. **CDN-hosted libraries**: GSAP and lite-youtube-embed via jsDelivr
2. **Lazy loading**: All images use `loading="lazy"`
3. **CSS optimization**: Inline styles for critical rendering path
4. **JavaScript efficiency**: Native APIs (Intersection Observer) instead of heavy libraries
5. **Image optimization**: Use WebP with JPEG fallbacks
6. **No build tools**: Direct file serving = instant load

## 🔍 SEO Features

- ✅ Meta tags for all languages with language variants (hreflang)
- ✅ Open Graph tags for social sharing
- ✅ JSON-LD structured data for MusicGroup schema
- ✅ XML sitemap with priority levels
- ✅ robots.txt for search engine crawling
- ✅ Semantic HTML5 structure
- ✅ Mobile-responsive viewport meta tag
- ✅ Descriptive title and meta descriptions

### Monitor SEO Performance

- Google Search Console: `https://search.google.com/search-console`
- Google PageSpeed Insights: `https://pagespeed.web.dev/`
- Microsoft Bing Webmaster Tools: `https://www.bing.com/webmasters`

## 📱 Browser Support

- Chrome/Edge: ✅ Latest
- Firefox: ✅ Latest
- Safari: ✅ Latest (11+)
- Mobile browsers: ✅ All modern

## 🎯 Booking System

The site uses two contact methods:

1. **WhatsApp (Primary)** - Click the button to start a chat with pre-filled message
2. **Email (Secondary)** - Opens default email client with booking subject

Messages are automatically translated based on selected language.

## 📈 Analytics Setup (Optional)

To add Google Analytics:

1. Create a Google Analytics account
2. Add this to the `<head>` section of `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your actual measurement ID.

## 🐛 Troubleshooting

### Site not loading after push
- Wait 5-10 minutes for GitHub Pages to rebuild
- Check repository settings are configured correctly
- Verify CNAME file exists with correct domain

### Custom domain not working
- DNS changes can take 24-48 hours
- Use `nslookup brazooca.com` to verify propagation
- Check domain registrar DNS settings

### Language not persisting
- Clear browser cache (localStorage)
- Language preference is saved in localStorage

### Videos not playing
- Check YouTube video ID is correct and video is public
- lite-youtube-embed loads on click (not autoplay)

## 📝 License

All content created for Brazooca Rock Club. Commercial use without permission prohibited.

## 👨‍💼 Contact

For booking inquiries, use WhatsApp or email from the website.

---

**Last Updated**: February 21, 2026  
**Hosted on**: GitHub Pages  
**Domain**: brazooca.com
Brazooca Rock Club
