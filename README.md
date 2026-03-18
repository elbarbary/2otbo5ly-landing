# 2otbo5ly Landing Page

A modern, animated landing page for 2otbo5ly - connecting home chefs with food lovers in Egypt.

## 🎨 Design Features

### Color Scheme
- **Primary Burgundy**: `#800020`
- **Light Burgundy**: `#A0334D`
- **Dark Burgundy**: `#5C0015`
- **Gold Accent**: `#D4AF37`
- **Warm Cream**: `#FFF8F6`

### Typography
- **Headings**: Playfair Display (serif) - elegant and premium
- **Body**: Inter (sans-serif) - clean and readable

### Hero Animation
The hero section features a sophisticated 14-second animation loop:

1. **Phase 1 (0-35%)**: TikTok-style food video on phone
   - Hawawshi (🫕) food emoji bouncing
   - Floating hearts with engagement metrics
   - User character watches intently

2. **Phase 2 (35-55%)**: Chef arrives with magic
   - Chef enters from right with magic wand sparkles
   - Phone glows with burgundy and gold light
   - User gets surprised

3. **Phase 3 (55-80%)**: Magical transformation
   - Phone shrinks and spins away (360° rotation)
   - Magic ring expansion effect
   - Giant hawawshi plate materializes with steam

4. **Phase 4 (80-100%)**: Celebration
   - Sparkle burst effect
   - User bounces excitedly
   - Chef presents proudly

## 📱 Responsive Design

- **Desktop** (900px+): Full animation with all details
- **Tablet** (600px-900px): Optimized spacing, nav links hidden
- **Mobile** (< 600px): Compact phone (140px × 280px), smaller TikTok elements

## 🚀 Deployment

### Option 1: Cloudflare Pages (Recommended)

1. **Connect your GitHub repository**
   ```bash
   gh repo view --web
   ```
   Visit your repository on GitHub.

2. **Go to Cloudflare Dashboard**
   - Log in to [dash.cloudflare.com](https://dash.cloudflare.com)
   - Go to **Pages** in the left sidebar
   - Click **Create a project** → **Connect to Git**

3. **Select Your Repository**
   - Choose `2otbo5ly-landing`
   - Select branch: `main` (or your preferred branch)

4. **Configure Build Settings**
   - **Build command**: Leave empty (static site)
   - **Build output directory**: `/` (root)
   - No build dependencies needed

5. **Deploy**
   - Click **Save and Deploy**
   - Cloudflare will deploy your site automatically
   - Get a free `*.pages.dev` subdomain

6. **Custom Domain (Optional)**
   - Go to **Custom domain** in Pages settings
   - Add your domain and follow DNS instructions

### Option 2: Cloudflare Workers (Advanced)

1. **Install Wrangler CLI**
   ```bash
   npm install -g @cloudflare/wrangler
   wrangler login
   ```

2. **Create `wrangler.toml`**
   ```toml
   name = "2otbo5ly-landing"
   type = "javascript"
   main = "src/index.js"

   [env.production]
   routes = [{pattern = "example.com/*", zone_name = "example.com"}]
   ```

3. **Deploy**
   ```bash
   wrangler publish
   ```

### Option 3: GitHub Pages

1. **Push to GitHub**
   ```bash
   git push origin main
   ```

2. **Enable in Repository Settings**
   - Go to repo **Settings** → **Pages**
   - Select **Source**: Deploy from a branch
   - Select branch: `main`
   - Select folder: `/ (root)`
   - Click **Save**

3. **Your site is live at**
   ```
   https://elbarbary.github.io/2otbo5ly-landing
   ```

## 🛠 Local Development

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- (Optional) Local web server for testing

### Run Locally

1. **Using Python 3**
   ```bash
   python -m http.server 8000
   ```
   Visit `http://localhost:8000`

2. **Using Node.js (http-server)**
   ```bash
   npx http-server
   ```

3. **Using VS Code Live Server**
   - Install extension "Live Server"
   - Right-click `index.html` → "Open with Live Server"

## 📊 Performance

- **Single HTML file**: No build process needed
- **CSS-only animations**: Smooth 60fps performance
- **Optimized SVG**: Lightweight vector graphics
- **Google Fonts**: Preconnected for fast loading
- **Responsive**: Mobile-first design

## 🎯 Features

- ✅ Fully responsive design
- ✅ Smooth CSS animations
- ✅ Intersection Observer for scroll effects
- ✅ Glassmorphism UI elements
- ✅ Bilingual support (English + Arabic)
- ✅ Accessible HTML structure
- ✅ No JavaScript dependencies

## 📝 Content Sections

1. **Navigation**: Fixed header with logo and CTA button
2. **Hero**: Animated character scene with TikTok transformation
3. **How It Works**: 3-step process with hover effects
4. **Reviews**: Scrolling testimonial cards with ratings
5. **Stats**: Key metrics display
6. **Download CTA**: App store links with animated orbs
7. **Footer**: Copyright and branding

## 🔧 Customization

### Colors
Edit CSS variables in the `:root` section:
```css
:root {
  --b:     #800020;  /* Primary burgundy */
  --bl:    #A0334D;  /* Light burgundy */
  --gold:  #D4AF37;  /* Gold accent */
  /* ... more colors ... */
}
```

### Animation Timing
Change the loop duration (default: 14s):
```css
:root {
  --loop: 14s;
}
```

### Fonts
Update Google Fonts imports and font-family declarations:
```css
font-family: 'Playfair Display', serif;  /* Headings */
font-family: 'Inter', system-ui, sans-serif;  /* Body */
```

## 📄 License

All rights reserved. © 2026 2otbo5ly

## 🤝 Support

For issues or questions, open a GitHub issue or contact the team.

---

**Last Updated**: March 2026
**Built with**: HTML5, CSS3, vanilla JavaScript
