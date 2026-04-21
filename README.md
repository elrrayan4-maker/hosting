# NexusHost — Game Server Hosting Website v3.0

A complete, production-ready game server hosting website with full admin panel.

## 📁 Project Structure

```
nexushost/
├── index.html      Main landing page (full site)
├── games.html      Complete games catalog (30+ games)
├── admin.html      Admin panel (manage everything)
├── styles.css      Global design system CSS
├── 404.html        Custom 404 error page
└── README.md       This file
```

## 🚀 Quick Start

### Option 1 — Local (No server needed)
Simply open `index.html` in any modern browser.

### Option 2 — GitHub Pages (Free hosting)
1. Create a GitHub account at github.com
2. Create a new repository (public)
3. Upload all files to the repository
4. Go to Settings → Pages → Deploy from Branch (main)
5. Your site is live at `https://yourusername.github.io/repo-name`

### Option 3 — Netlify (Recommended, Free)
1. Go to netlify.com → Sign up free
2. Drag & drop the entire project folder onto the Netlify dashboard
3. Your site is instantly live with a `.netlify.app` URL
4. Connect a custom domain in Settings

### Option 4 — Vercel (Free)
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the project folder
3. Follow prompts — live in seconds

### Option 5 — Any Web Host (cPanel/FTP)
Upload all files to your `public_html` folder via FTP or the file manager.

## ⚙️ Configuration

All site content is managed through the **Admin Panel** (`admin.html`).

### Admin Login
- **URL:** `yoursite.com/admin.html`
- **Default username:** `admin`
- **Default password:** `nexushost2025`
- **Change password** in Admin → Settings → Change Password

### Discord Webhook Setup
1. In Discord, right-click your channel → Edit Channel → Integrations → Webhooks
2. Create a new webhook and copy the URL
3. In Admin → Webhook Config, paste the URL and click Save
4. Click "Send Test" to verify it works

You'll receive Discord notifications for:
- New orders
- New support tickets
- Admin replies to tickets

### Customizing Content (Admin Panel)
| Section | Admin Page | What you can edit |
|---------|-----------|-------------------|
| Hero text | Site Content | Headlines, badge text, description |
| Site name & logo | Site Content | Name, logo text, copyright, footer |
| Game cards | Games Manager | Photos, names, tags, visibility |
| Plans | Plans Editor | Price, RAM, CPU, storage, photos, extras |
| Features | Features Editor | Icons, titles, descriptions |
| Testimonials | Testimonials | Reviews, names, colors, ratings |

## 📱 Mobile Support
- Fully responsive from 320px to 4K
- Touch-friendly hamburger navigation
- Bottom-sheet modals on mobile
- `viewport-fit=cover` for iPhone notch

## 🌐 SEO & Performance
- Open Graph meta tags for social sharing
- Theme color for browser chrome
- `loading="lazy"` on all images
- `prefers-reduced-motion` support
- Semantic HTML with ARIA roles

## 🔒 Security Notes
- All data stored in browser `localStorage`
- No backend required for basic operation
- For production: replace localStorage with a real backend API
- Admin panel uses client-side auth (upgrade for production)

## 📊 Data Storage (localStorage keys)
| Key | Contents |
|-----|----------|
| `nexushost_config` | All site config (plans, games, content) |
| `nexushost_orders` | Customer orders |
| `nexushost_tickets` | Support tickets |
| `nexushost_users` | Registered user accounts |
| `nexushost_user` | Currently logged in user |
| `nexushost_webhook` | Discord webhook URL |
| `nexushost_admin_creds` | Admin login credentials |

## 🎨 Design System
The `styles.css` file contains a complete design system:
- CSS custom properties (variables) for all colors, spacing, radius
- Responsive utility classes
- Pre-built button, badge, card, modal, form components
- Scroll reveal animations
- Mobile-first breakpoints

## 📞 Support
For questions or issues with this template, open a ticket in the Admin Panel.

---
Built with ❤️ by NexusHost
