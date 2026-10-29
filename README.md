# MD Sojibor Rahman - Portfolio Website

Personal portfolio website for **MD Sojibor Rahman** — WordPress Developer, Photographer, and Textile Engineer based in Dhaka, Bangladesh.

Built with **Midnight Amber** theme, DaisyUI, Tailwind CSS, Google Fonts (*Playfair Display* & *Inter*), smooth scroll animations via `IntersectionObserver`, hero typing effects, photography lightbox, and dark/light mode toggle with `localStorage` persistence.

---

## 🚀 How to Deploy from GitHub to Vercel (Step-by-Step)

### Step 1: Create a GitHub Repository
1. Go to [GitHub](https://github.com/) and sign in.
2. Click the **`+`** icon in the top-right corner and select **New repository**.
3. Name your repository (e.g. `sojibor-portfolio`).
4. Set it to **Public** (or **Private**).
5. Do **not** initialize with README, .gitignore, or license (we already have them here).
6. Click **Create repository**.

---

### Step 2: Push this Project to GitHub
In your local terminal inside the project root folder, run:

```bash
# Initialize git
git init

# Add all files
git add .

# Make your initial commit
git commit -m "Initial commit: MD Sojibor Rahman portfolio"

# Set main branch
git branch -M main

# Link to your GitHub repo (replace YOUR_USERNAME and YOUR_REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push code to GitHub
git push -u origin main
```

---

### Step 3: Deploy to Vercel (Free & Instant)
1. Go to [Vercel](https://vercel.com/) and sign up or log in (you can sign in directly with GitHub).
2. On your Vercel Dashboard, click **Add New...** → **Project**.
3. Under **Import Git Repository**, find your repo (`sojibor-portfolio`) and click **Import**.
4. In the **Configure Project** screen:
   - **Framework Preset**: Vite *(Vercel will auto-detect this via `vercel.json`)*
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
5. Click **Deploy**.

---

### 🎉 Result
In about 20-30 seconds, Vercel will build and assign you a free production URL (e.g., `https://sojibor-portfolio.vercel.app`).
Every time you push changes to GitHub, Vercel will automatically redeploy your live website!

---

### 🌐 Structure & Dedicated Pages
- **`index.html`**: Main landing page with dynamic Hero, About, Selected Web Work, BUTEX Research, Photography Preview, Services, and Contact.
- **`work.html`**: Dedicated "All Web Work & Case Studies" directory with live search, category filtering, and **Excel / Google Sheets sync**.
- **`gallery.html`**: Dedicated "Photography & Visual Archives" gallery with live search, category filtering, fullscreen lightbox, and **Excel / Google Sheets sync**.

---

## 📊 How to Connect Your 2 Google Sheets / Excel Spreadsheets

### For Previous Web Work (`work.html`):
1. In Google Sheets, make columns: `Title, Category, Challenge, Solution, Result, Tech, ImageUrl`
2. Go to **File → Share → Publish to web**.
3. Select **Comma-separated values (.csv)** and click **Publish**.
4. Copy the link, go to `/work.html`, click **Connect Excel / Sheet**, paste the link, and click **Fetch**!
*(Or click "Download Excel Template" to edit locally and upload `.xlsx`)*

### For Photography (`gallery.html`):
1. In Google Sheets, make columns: `Title, Category, Caption, Location, Gear, FullImageUrl, ThumbnailUrl`
2. Publish to web as **CSV**.
3. Go to `/gallery.html`, click **Connect Excel / Sheet**, paste the link, and click **Fetch**!
*(Or upload an `.xlsx` file directly)*

