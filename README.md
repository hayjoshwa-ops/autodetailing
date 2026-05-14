# 🌿 Neighbourhood Pro

> **Your Friendly Neighbourhood Service Hub** — Yard Maintenance · Auto Detailing · Tech Help

A full-featured, multi-service web application built for a local neighbourhood service business. Three distinct service lines, each with its own branded dark-themed page, unified under one clean main app shell. Built with React + Vite and ready to deploy to Netlify in minutes.

---

## 📸 Services

### 🌿 Yard Maintenance
Dark olive + gold theme. Covers lawn mowing, weed & edging, and general yard upkeep (not hardscaping or full installs). Includes a how-it-works flow, customer reviews, and quote request CTA.

### 🚗 Auto Detailing — Haywood & Sons
Dark navy + electric blue chrome theme. Features the real Haywood & Sons logo, three detail packages (Express, Full, Premium), monthly maintenance plans (Express / Full / Premium), add-ons, and customer reviews. All prices are **starting rates** confirmed after inspection.

### 💻 Tech Help
Dark purple + violet theme. Covers Apple support (Mac, iPhone, iPad), PC repair (Windows, virus removal, hardware), and custom PC builds (Budget → High-End). Includes a common fixes pricing table and build tier cards.

---

## ✨ Features

- **Three full-page service experiences** — each with its own font, color palette, and layout
- **Smart booking flow** — selecting a package pre-fills and locks the contact form so customers can't accidentally book the wrong service
- **Live review system** — customers leave reviews that render instantly with color-coded cards (green = lawn, blue = auto, purple = tech)
- **Before & after gallery** — flip cards showing job transformations
- **Auto detailing package picker** — radio-button style package selector inside the contact form when "Auto Detailing" is chosen
- **Tech Help contact prompt** — special info block appears when a tech service is selected, prompting customers to describe their issue
- **Form validation** — both the review form and booking form show clear error messages when required fields are empty
- **Clickable phone number** — `(208) 640-1855` is tappable everywhere (header, footer, CTA banners)
- **Fully mobile responsive** — tested on iPhone screen widths

---

## 🛠 Tech Stack

| Layer | Tool |
|-------|------|
| Framework | [React 18](https://react.dev) |
| Build Tool | [Vite 5](https://vitejs.dev) |
| Styling | Inline React styles (no CSS framework dependency) |
| Fonts | Google Fonts (Playfair Display, Orbitron, Rajdhani, Cinzel, Lato, Share Tech Mono) |
| Deployment | [Netlify](https://netlify.com) (recommended) |
| Forms (planned) | [Formspree](https://formspree.io) |
| Database (planned) | [Supabase](https://supabase.com) |

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org) v18+ (LTS recommended)
- npm (comes with Node)

### Install & Run

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/neighbourhood-pro.git
cd neighbourhood-pro

# 2. Install dependencies
npm install

# 3. Start the dev server
npm run dev
```

Then open **http://localhost:5173** in your browser.

### Build for Production

```bash
npm run build
```

Output goes to the `dist/` folder — ready to drag onto Netlify.

---

## 📁 Project Structure

```
neighbourhood-pro/
├── index.html              # App entry point
├── vite.config.js          # Vite configuration
├── package.json
└── src/
    ├── main.jsx            # React root mount
    └── App.jsx             # Full application (single-file architecture)
        ├── YardPage        # Yard maintenance full-page component
        ├── AutoPage        # Auto detailing full-page component
        ├── TechPage        # Tech help full-page component
        └── App (default)   # Main shell: Home, Services, Gallery, Reviews, Contact
```

---

## 🧭 App Navigation

```
Home
├── Yard Maintenance  →  YardPage (dark olive/gold)
├── Auto Detailing    →  AutoPage (dark navy/blue)
└── Tech Help         →  TechPage (dark purple)

Services             →  Two banner cards linking to sub-pages
Gallery              →  Before/after flip cards
Reviews              →  Live review submission + color-coded display
Contact / Book       →  Smart booking form with package pre-fill
```

---

## 🎨 Design System

Each service has its own isolated color palette:

| Service | Background | Accent | Font |
|---------|-----------|--------|------|
| Main App | `#f7f4ee` warm cream | `#2d6a4f` forest green | Playfair Display |
| Yard Maintenance | `#0c110a` dark olive | `#c9a227` gold | Cinzel + Lato |
| Auto Detailing | `#080e1a` midnight navy | `#4db8ff` electric blue | Orbitron + Rajdhani |
| Tech Help | `#0e0a1a` deep purple | `#a78bfa` violet | Share Tech Mono + Inter |

---

## 📋 Pricing (Auto Detailing)

| Package | Sedan | SUV/Truck |
|---------|-------|-----------|
| Express Detail | Starting at $75 | Starting at $95 |
| Full Detail ⭐ | Starting at $200 | Starting at $250 |
| Premium Detail | Starting at $250 | Starting at $350 |

**Monthly Plans:** Express $79/mo · Full $119/mo · Premium $179/mo

**Add-ons:** Pet Hair Removal $25+ · Stain Treatment $25+

> All prices are starting rates. Final pricing confirmed after vehicle inspection.

---

## 📞 Contact

**Haywood & Sons — Car Wash & Detailing**
📞 (208) 640-1855

---

## 🗺 Roadmap

- [ ] **Formspree integration** — booking form emails owner on submission
- [ ] **Supabase backend** — persistent reviews stored in a real database
- [ ] **Custom domain** — `haywoodandsonspro.com` or similar via Namecheap
- [ ] **Netlify deploy** — drag-and-drop `dist/` folder for live URL
- [ ] **Photo uploads** — real before/after customer photos in the gallery
- [ ] **Online scheduling** — Calendly or Square Appointments integration
- [ ] **Google Reviews embed** — pull live reviews from Google Business Profile
- [ ] **SMS notifications** — Twilio integration for booking alerts

---

## 🚢 Deploying to Netlify (Free)

1. Run `npm run build`
2. Go to [netlify.com](https://netlify.com) → sign up free
3. Drag the `dist/` folder onto the Netlify dashboard
4. Your site is live at a `*.netlify.app` URL instantly
5. Optionally connect a custom domain in Netlify settings

---

## 📄 Assets

| File | Description |
|------|-------------|
| `haywood_price_sheet.pdf` | Auto detailing price sheet (dark navy theme) |
| `haywood_price_sheet.png` | Price sheet as a shareable image (1700×2200px) |
| `haywood_price_sheet.txt` | Plain text version for SMS / messaging |

---

## 📝 License

Private — All rights reserved. Built for Haywood & Sons / Neighbourhood Pro.

---

*Built with ❤️ using React + Vite*
