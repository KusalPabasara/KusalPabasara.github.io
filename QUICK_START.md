# Quick Start Guide - Portfolio Website

## 🚀 Viewing Your Portfolio

### Local Preview
Your website is currently running at: **http://localhost:8000**

To stop the server:
```bash
# Find the process and stop it
pkill -f "python3 -m http.server"
```

To start again:
```bash
cd /home/kusal/MYPersonalWebsite
python3 -m http.server 8000
```

---

## 📤 Deployment Options

### Option 1: GitHub Pages (Recommended - FREE)

1. **Create a GitHub repository** (if not already done)
2. **Push your code:**
   ```bash
   cd /home/kusal/MYPersonalWebsite
   git add .
   git commit -m "Updated portfolio with DaisyUI and achievements"
   git push origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Settings → Pages
   - Source: Deploy from branch "main"
   - Select root folder
   - Save

Your site will be available at: `https://kusalpabasara.github.io/MYPersonalWebsite/`

### Option 2: Netlify (FREE)

1. Go to [netlify.com](https://netlify.com)
2. Sign in with GitHub
3. Click "Add new site" → "Import an existing project"
4. Select your GitHub repository
5. Deploy!

Your site will be available at: `https://your-site-name.netlify.app`

### Option 3: Vercel (FREE)

1. Go to [vercel.com](https://vercel.com)
2. Sign in with GitHub
3. Click "New Project"
4. Import your repository
5. Deploy!

Your site will be available at: `https://your-site-name.vercel.app`

---

## ✨ Customization Tips

### 1. Change Colors
Edit the `:root` section in the `<style>` tag:
```css
:root {
    --primary-color: rgb(2, 82, 255);  /* Change this */
    --secondary-color: #5070d8;         /* And this */
    --dark-color: #2b3d5b;
    --light-color: #f8fafc;
}
```

### 2. Update Contact Form
The form currently uses Formspree: `https://formspree.io/f/xvgkbwnv`

To use your own:
1. Go to [formspree.io](https://formspree.io)
2. Create a new form
3. Replace the action URL in both forms in index.html

### 3. Add More Projects
Find this section and duplicate the `project-card` div:
```html
<!-- Hackathon Achievements Section -->
<section class="projects" id="achievements">
```

### 4. Update CV
Simply replace `CV.pdf` with your latest resume file (keep the same name).

---

## 🎨 DaisyUI Themes

Want to change the theme? Add this to your `<html>` tag:

Available themes:
- `data-theme="light"` (current)
- `data-theme="dark"`
- `data-theme="cupcake"`
- `data-theme="bumblebee"`
- `data-theme="emerald"`
- `data-theme="corporate"`
- `data-theme="synthwave"`
- `data-theme="retro"`
- `data-theme="cyberpunk"`
- `data-theme="valentine"`
- `data-theme="halloween"`
- `data-theme="garden"`
- `data-theme="forest"`
- `data-theme="aqua"`
- `data-theme="lofi"`
- `data-theme="pastel"`
- `data-theme="fantasy"`
- `data-theme="wireframe"`
- `data-theme="black"`
- `data-theme="luxury"`
- `data-theme="dracula"`

Example:
```html
<html lang="en" data-theme="dark">
```

---

## 📱 Social Media Updates

Don't forget to update these:
1. LinkedIn profile link
2. GitHub profile link
3. Instagram link
4. Facebook link

All are already configured in your footer and contact sections!

---

## 🔍 SEO Tips

1. **Add a meta description** in the `<head>`:
   ```html
   <meta name="description" content="Kusal Pabasara - Computer Science student, Hackathon Champion, ML enthusiast">
   ```

2. **Add Open Graph tags** for social media sharing:
   ```html
   <meta property="og:title" content="Kusal Pabasara | CS Undergraduate">
   <meta property="og:description" content="Hackathon Champion | ML & Data Science Enthusiast">
   <meta property="og:image" content="MyImage.png">
   ```

3. **Add a favicon**:
   ```html
   <link rel="icon" type="image/png" href="favicon.png">
   ```

---

## 📊 Analytics (Optional)

Add Google Analytics to track visitors:

1. Create account at [analytics.google.com](https://analytics.google.com)
2. Get your tracking ID
3. Add this before `</head>`:
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

---

## 🐛 Troubleshooting

### Images not loading?
- Check file names match exactly (case-sensitive)
- Ensure images are in the same folder as index.html

### CV not downloading?
- Make sure CV.pdf is in the root folder
- Try right-click → "Save link as" if automatic download fails

### Forms not working?
- Check Formspree URL is correct
- Ensure you're connected to the internet
- Check browser console for errors (F12)

---

## 📞 Need Help?

Check these resources:
- DaisyUI Docs: https://daisyui.com/
- Tailwind CSS: https://tailwindcss.com/
- Font Awesome Icons: https://fontawesome.com/icons

---

**Happy Coding! 🚀**

Your portfolio is now professional, modern, and showcases your amazing achievements!
