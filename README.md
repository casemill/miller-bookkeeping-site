# Miller Bookkeeping Website

A professional, responsive website for Miller Bookkeeping built with Next.js 15, featuring a custom SVG logo and modern design.

## 🌐 Live Website
**Current Live Site:** https://same-gsqph237d6e-latest.netlify.app

## 🚀 Quick Start for Local Development

### Prerequisites
- **Node.js** (v18 or higher)
- **Bun** (recommended) or npm
- **Git**
- Your favorite code editor (VS Code, Sublime Text, etc.)

### 1. Clone the Repository
```bash
git clone https://github.com/casemill/miller-bookkeeping-site.git
cd miller-bookkeeping-site
```

### 2. Install Dependencies
```bash
bun install
# or
npm install
```

### 3. Start Development Server
```bash
bun dev
# or
npm run dev
```

Visit `http://localhost:3000` to see your site locally.

## 📝 Making Changes

### Key Files to Edit:

#### **`src/lib/config.ts`** - Main Customization File
This is your one-stop file for customizing all content:
```typescript
// Business Information
business: {
  name: "Miller Bookkeeping",
  tagline: "Professional Accounting Services",
  description: "Your trusted partner for bookkeeping...",
},

// Contact Information
contact: {
  email: "info@millerbooks.com",
  phone: "(555) 123-4567",
  address: "123 Business St, Your City, State 12345",
},
```

#### **`public/logo.svg`** - Your Logo
Replace this file with your updated logo (keep the filename the same).

#### **`src/components/`** - Individual Page Sections
- `Header.tsx` - Navigation and logo
- `Hero.tsx` - Main banner section
- `MainContent.tsx` - Article content area
- `Footer.tsx` - Footer with contact info

## 🔄 Deployment Workflow

### Automatic Deployment (Recommended)
1. **Make changes** locally in your editor
2. **Test locally** with `bun dev`
3. **Commit changes**:
   ```bash
   git add .
   git commit -m "Description of your changes"
   ```
4. **Push to GitHub**:
   ```bash
   git push origin main
   ```
5. **Netlify automatically deploys** your changes within 1-2 minutes!

### Manual Deployment (Alternative)
- Build your site: `bun run build`
- Upload the `out/` folder contents to Netlify dashboard

## 🛠️ Common Customizations

### Update Business Information
Edit `src/lib/config.ts` and change:
- Business name and tagline
- Contact information (email, phone, address)
- Social media links
- Navigation menu items

### Change Colors/Styling
- Edit `src/app/globals.css` for global styles
- Modify Tailwind classes in component files
- Update color schemes in individual components

### Add New Pages
1. Create new file in `src/app/[page-name]/page.tsx`
2. Add navigation link in `src/lib/config.ts`
3. Create corresponding component if needed

### Replace Images
- Logo: Replace `public/logo.svg`
- Hero background: Update URL in `src/lib/config.ts`
- Content images: Add to `public/` folder and reference in config

## 📁 Project Structure
```
├── public/
│   └── logo.svg                    # Your business logo
├── src/
│   ├── app/
│   │   ├── globals.css            # Global styles
│   │   ├── layout.tsx             # App layout
│   │   └── page.tsx               # Home page
│   ├── components/
│   │   ├── Header.tsx             # Navigation header
│   │   ├── Hero.tsx               # Hero banner
│   │   ├── MainContent.tsx        # Main content area
│   │   ├── Footer.tsx             # Footer section
│   │   └── ui/                    # Reusable UI components
│   └── lib/
│       └── config.ts              # 🎯 MAIN CUSTOMIZATION FILE
├── netlify.toml                   # Netlify deployment config
├── next.config.js                 # Next.js configuration
└── package.json                   # Dependencies and scripts
```

## 🔧 Available Scripts

- `bun dev` - Start development server
- `bun build` - Build for production
- `bun start` - Start production server
- `bun lint` - Run linting

## 📞 Support

For technical issues or customization help:
- Check this README first
- Review the `src/lib/config.ts` file
- Test changes locally before pushing
- Contact your developer if needed

## 🎨 Features

- ✅ **Responsive Design** - Works on all devices
- ✅ **Custom Logo Integration** - Your BOOKKEEPING logo at 240px width
- ✅ **Professional Layout** - Header, hero, content, footer
- ✅ **Easy Customization** - Central config file
- ✅ **Fast Loading** - Optimized static site
- ✅ **SEO Friendly** - Proper meta tags and structure
- ✅ **Automatic Deployment** - Git push = live updates

---

**Built with:** Next.js 15, TypeScript, Tailwind CSS, Bun
**Deployed on:** Netlify