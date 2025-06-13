# Le Panier de Saison - PWA Setup Guide

## 📱 PWA (Progressive Web App) Setup

Your HTML page has been transformed into a PWA! Here's what you need to complete the setup:

### 1. Create App Icons

You need to create two icon files with your app logo:

- `icon-192x192.png` (192x192 pixels)
- `icon-512x512.png` (512x512 pixels)

**Recommendations for icons:**
- Use a simple, recognizable design (maybe a basket with fruits/vegetables)
- Ensure the design is readable at small sizes
- Use your app's color scheme (#4A5C3D green and #FAF8F2 cream)
- You can use tools like [PWA Asset Generator](https://www.pwabuilder.com/imageGenerator) or create them manually

### 2. File Structure

Your project should have these files:
```
/
├── index.html          ✅ (updated with PWA features)
├── manifest.json       ✅ (created)
├── sw.js              ✅ (service worker created)
├── icon-192x192.png   ❌ (you need to create this)
└── icon-512x512.png   ❌ (you need to create this)
```

## 🌐 Hosting Options

### Option 1: GitHub Pages (Recommended - Free & Easy)

1. **Create a GitHub account** if you don't have one
2. **Create a new repository** named `seasonal-produce` (or any name you prefer)
3. **Upload all your files** to the repository
4. **Enable GitHub Pages:**
   - Go to repository Settings
   - Scroll to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Save
5. **Your site will be available at:** `https://yourusername.github.io/seasonal-produce`

### Option 2: Netlify (Free with drag & drop)

1. Go to [netlify.com](https://netlify.com)
2. Sign up for free
3. Drag and drop your folder to the deploy area
4. Get an instant URL like `https://amazing-name-123456.netlify.app`
5. **Optional:** Connect to GitHub for automatic updates

### Option 3: Vercel (Free, great performance)

1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub
3. Click "New Project"
4. Import your repository
5. Deploy automatically

### Option 4: Firebase Hosting

1. Install Firebase CLI: `npm install -g firebase-tools`
2. Run `firebase init hosting`
3. Deploy with `firebase deploy`

## 📱 PWA Features Added

- ✅ **Offline functionality** - Works without internet after first visit
- ✅ **Installable** - Shows install prompt on mobile/desktop
- ✅ **App-like experience** - Runs in standalone mode
- ✅ **Caching** - Fast loading with service worker
- ✅ **Mobile optimized** - Perfect for phones and tablets

## 🔧 Testing Your PWA

1. **Deploy your site** using one of the hosting options above
2. **Open in Chrome/Edge** on mobile or desktop
3. **Look for install prompt** - You should see a "📱 Installer l'application" button
4. **Test offline** - Disconnect internet and reload page
5. **Check PWA score** - Use Chrome DevTools Lighthouse audit

## 📝 Notes

- PWAs require HTTPS to work (all hosting options above provide this)
- The install prompt only appears on supported browsers (Chrome, Edge, Firefox)
- On iOS Safari, users can manually add to home screen via Share button
- The app will update automatically when you deploy changes

## 🎨 Customization

You can customize the PWA by editing `manifest.json`:
- Change app name, colors, or orientation
- Add more icons for different sizes
- Modify the start URL or scope

## 🚀 Next Steps

1. Create your app icons
2. Choose a hosting option and deploy
3. Test the PWA functionality
4. Share your app URL with users!

Your seasonal produce guide will now work like a native app on any device! 🥕🍎 