# Rosie Boi's Sliders — Website

Static HTML/CSS/JS website for Rosie Boi's Sliders food truck.

---

## 📁 File Structure

```
rosie-bois-sliders/
├── index.html       ← Main website (everything is in here)
├── logo.png         ← Rosie Boi's logo (keep in same folder as index.html)
└── README.md        ← This file
```

---

## 🚀 Option 1 — Host on GitHub Pages (Free)

1. Create a new GitHub repo (e.g. `rosie-bois-sliders`)
2. Upload `index.html` and `logo.png` to the root of the repo
3. Go to **Settings → Pages**
4. Set **Source** to `main` branch, folder `/root`
5. Click **Save**
6. Your site will be live at: `https://yourusername.github.io/rosie-bois-sliders`

---

## 🔗 Option 2 — Use with Go High Level (GHL)

### Method A: Embed as a Custom HTML Page (Recommended)

1. In GHL, go to **Sites → Funnels** or **Websites**
2. Create a new Funnel or Website
3. Add a new page step
4. Click **Edit** → switch to **Custom Code / HTML mode**
5. Paste the full contents of `index.html`
6. For the logo: upload `logo.png` to GHL's **Media Library**, copy the URL, then replace `logo.png` in the HTML with that full URL (search for `src="logo.png"` — there are 3 instances)
7. Save and publish

### Method B: Iframe from GitHub Pages into GHL

1. First deploy to GitHub Pages (Option 1 above)
2. In GHL, add an **HTML Element** to any page
3. Use this code:
```html
<iframe src="https://yourusername.github.io/rosie-bois-sliders" 
        width="100%" height="100vh" 
        style="border:none; min-height:100vh;">
</iframe>
```

---

## ✏️ How to Update Content

### Change menu prices or items
Open `index.html` and search for the item name. Each menu item looks like:
```html
<div class="menu-item">
  <div class="menu-item-top">
    <span class="item-name">Classic Rosie Slider</span>
    <span class="item-price">$5.00</span>
  </div>
  <p class="item-desc">Description here.</p>
</div>
```

### Change the truck schedule
Search for `schedule-row` — update the day and location text.

### Change social media links
Search for `Instagram`, `Facebook`, `TikTok` in the footer — update the `href="#"` with your real URLs.

### Change catering email
Search for `catering@rosieboissliders.com` — replace with your real email.

### Swap in real food photos
The site uses Unsplash photos. To use your own:
- Upload photos to GHL Media Library or any image host (Cloudinary, imgbb, etc.)
- Search `images.unsplash.com` in the HTML and replace each URL with your photo URL

---

## 🎨 Brand Colors

| Name    | Hex       |
|---------|-----------|
| Black   | `#0a0700` |
| Gold    | `#c9952a` |
| Red     | `#c0272d` |
| Cream   | `#f5e9c8` |
| Dark    | `#120d04` |

---

## 📞 Need Help?

To get more help customizing this site, just ask your web developer or reach back out to whoever built this.
