# 🍼 little names ✦

> A beautiful, private baby name suggestion & voting website for friends and family.

**[Live Demo →](https://YOUR-USERNAME.github.io/little-names)**

---

## ✨ Features

- **Anonymous submissions** — No login, no email, no tracking. Just names.
- **Multi-name input** — Submit multiple names at once, comma or line separated
- **Smart deduplication** — Same name submitted twice? The suggestion count goes up, not a duplicate
- **Community voting** — Everyone can vote for their favourite names with a heart
- **Browse & filter** — Filter by Boy / Girl / Neutral, sort by most voted, most suggested, A–Z, or newest
- **Live search** — Instant search across all submitted names
- **Parents' dashboard** — Private password-protected admin area with stats, management tools, and CSV export
- **Confetti celebration** — Delightful animation on every submission
- **Mobile-first** — Looks great on every device, from phones to desktops
- **Zero dependencies** — Pure HTML, CSS, and JavaScript. No frameworks, no build tools.
- **Works offline** — All data stored in the browser via localStorage

---

## 🚀 Deploy to GitHub Pages (5 minutes)

### Step 1 — Create a new GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Name it something like `little-names` or `baby-names`
3. Set it to **Public** (required for free GitHub Pages)
4. Click **Create repository**

### Step 2 — Upload the file

**Option A — Via GitHub web interface (easiest):**
1. On your new repo page, click **"uploading an existing file"**
2. Drag and drop `index.html` into the upload area
3. Click **Commit changes**

**Option B — Via Git (command line):**
```bash
git init
git add index.html
git commit -m "Initial commit — little names website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/little-names.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in the left sidebar)
3. Under **Source**, select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**

⏳ Wait 1–2 minutes, then your site will be live at:
```
https://YOUR-USERNAME.github.io/little-names
```

### Step 4 — Share the link!

Send the link to family and friends. That's it!

---

## 🔐 Admin Dashboard

The parents' dashboard is at the bottom of the navigation bar (the **"Parents ✦"** button).

**Default password:** `babynames2025`

Inside the dashboard you can:
- View all submitted names with vote and suggestion counts
- Remove inappropriate names
- Reset all votes
- Clear all names
- Export everything to a CSV spreadsheet
- Change the admin password

> **Important:** Change the default password after first login. The new password is stored in your browser's localStorage.

---

## 📱 Mobile Support

The site is fully responsive and works beautifully on:
- iPhone / Android phones
- Tablets
- Desktop browsers

It also works as a PWA (Progressive Web App) — visitors on mobile can "Add to Home Screen" for an app-like experience.

---

## 💾 Data Storage

All data (names, votes) is stored in the browser's **localStorage**.

**What this means:**
- ✅ Zero cost — no server or database needed
- ✅ Instant — no loading times
- ✅ Private — data stays in each person's browser
- ⚠️ Not shared across devices by default

**For a family website**, this works perfectly — each visitor sees and votes on the names, and their votes persist on their own device.

> If you want shared/synced data across all visitors, you would need to add a backend (Firebase, Supabase, etc.). The code is structured to make this easy to add.

---

## 🎨 Customisation

All the easy customisations are at the top of `index.html`:

### Change the site name / message
Search for `little names` and replace with your own name.

Change the hero headline:
```html
<h1 class="serif">Help Us Choose the<br><em>Perfect Baby Name</em></h1>
```

Change the subheadline:
```html
<p class="hero-sub">Your custom message here...</p>
```

### Change the colour scheme
Edit the CSS variables at the top of the `<style>` block:
```css
:root {
  --sage:       #7A9E7E;   /* Main accent colour */
  --sage-dark:  #4A6B4E;   /* Buttons & headings */
  --gold:       #C4A45A;   /* Gold accents */
  /* etc. */
}
```

### Change the admin password (in code)
Find this line in the `<script>` block:
```js
function getAdminPw() {
  return localStorage.getItem(PW_KEY) || 'babynames2025';
}
```
Replace `'babynames2025'` with your own default password.

---

## 🛠️ Tech Stack

| Layer | Tech |
|-------|------|
| HTML | Semantic HTML5 |
| CSS | Custom properties, CSS Grid, Flexbox |
| JS | Vanilla ES6+ (no framework) |
| Fonts | Google Fonts (Playfair Display + DM Sans) |
| Storage | Browser localStorage |
| Hosting | GitHub Pages (static) |

**No build step. No Node.js. No npm. Just one HTML file.**

---

## 📄 Licence

Free to use for personal use. Made with love ♡
