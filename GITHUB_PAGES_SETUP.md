# 🌐 GitHub Pages Setup Guide

## Quick Setup (5 Minutes)

### Step 1: Create New Repository
1. Go to GitHub: https://github.com/new
2. Repository name: `phantom-ai-website` (or any name)
3. Set to **Public**
4. ✅ Check "Add a README file"
5. Click **Create repository**

### Step 2: Upload index.html
1. In your new repository, click **Add file** → **Upload files**
2. Drag and drop `index.html` from your desktop
3. Commit: "Add PHANTOM AI landing page"
4. Click **Commit changes**

### Step 3: Enable GitHub Pages
1. Go to repository **Settings**
2. Scroll down to **Pages** (left sidebar)
3. Under "Source":
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **Save**
5. Wait 2-3 minutes for deployment

### Step 4: Get Your Website URL
Your website will be live at:
```
https://YOUR_USERNAME.github.io/phantom-ai-website/
```

Example: `https://sainionhacks.github.io/phantom-ai-website/`

---

## 📹 Adding Video Demo (When Ready)

### Option 1: YouTube (Recommended)
1. Upload video to YouTube
2. Get embed code: Video → Share → Embed
3. In `index.html`, find line **~398**:
```html
<div class="video-placeholder">
    📹 Video Demo Coming Soon!
</div>
```

4. Replace with:
```html
<iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID" 
        allowfullscreen></iframe>
```

### Option 2: Direct Upload
```html
<video controls style="width:100%; border-radius:10px;">
    <source src="demo-video.mp4" type="video/mp4">
</video>
```

---

## ⬇️ Adding EXE Download (When Ready)

### Step 1: Create GitHub Release
1. Go to repository → **Releases** → **Create a new release**
2. Tag: `v2.1`
3. Title: `PHANTOM AI v2.1 - Windows`
4. Upload `Phantom-AI.exe`
5. Click **Publish release**

### Step 2: Update Download Link
In `index.html`, find line **~574**:
```html
<a href="#" class="download-button disabled">
```

Replace with:
```html
<a href="https://github.com/YOUR_USERNAME/phantom-ai-website/releases/download/v2.1/Phantom-AI.exe" 
   class="download-button">
```

Remove `disabled` class to enable the button.

---

## 🎨 Customization

### Change Contact Email
Find all instances of `nitinsaini077@gmail.com` and replace with your email.

### Update Repository Links
Replace `SainiONHacks/phantom-ai-licenses` with your license repo.

### Modify Pricing
Edit the pricing cards section (lines ~420-520):
```html
<div class="price">₹100</div>
```

---

## 🔧 Maintenance

### Update Content
1. Edit `index.html` locally
2. Push to GitHub: `git add index.html && git commit -m "Update" && git push`
3. Changes appear in 1-2 minutes

### Check Analytics
Add Google Analytics by adding before `</head>`:
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

## 📱 Mobile Optimization
The page is already mobile-responsive! Test on phones/tablets.

---

## 🎯 SEO Optimization (Optional)

Add to `<head>` section for better Google ranking:
```html
<meta property="og:title" content="PHANTOM AI - Ultimate AI Assistant">
<meta property="og:description" content="AI-powered assistant for interviews, research & productivity">
<meta property="og:image" content="https://your-site.com/preview-image.png">
<meta property="og:url" content="https://your-site.com">
<meta name="twitter:card" content="summary_large_image">
```

---

## 🚀 Custom Domain (Optional)

1. Buy domain from Namecheap/GoDaddy
2. Add `CNAME` file to repository:
   ```
   phantom-ai.com
   ```
3. Update DNS records:
   - Type: `CNAME`
   - Name: `www`
   - Value: `YOUR_USERNAME.github.io`

---

## ✅ Checklist Before Launch

- [ ] Test all "Buy Now" email links
- [ ] Verify GitHub license repo link
- [ ] Test website on mobile
- [ ] Add video demo when ready
- [ ] Upload EXE and update download link
- [ ] Test all navigation links
- [ ] Check all sections load properly

---

## 📞 Need Help?

- GitHub Pages Docs: https://docs.github.com/pages
- Contact: nitinsaini077@gmail.com

---

**Pro Tip:** Share your website URL in:
- LinkedIn posts
- Twitter/X
- Reddit (r/SideProject, r/indiehackers)
- Product Hunt
- Email signature

Your website: `https://YOUR_USERNAME.github.io/phantom-ai-website/`
