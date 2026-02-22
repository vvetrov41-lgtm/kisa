# Kristina Vishar — Portfolio Website

Premium single-page portfolio for **Kristina Vishar (KV.)**, colour tattoo artist based in Manchester, UK.

**Stack:** Pure HTML + CSS + Vanilla JS (no build tools required)

---

## Local Preview

Just open `index.html` in any browser. All assets are local.

---

## Deploy to GitHub + Cloudflare Pages

### Step 1 — Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Name: `kristina-vishar-portfolio` (or any name)
3. Visibility: **Public** or **Private** (both work with Cloudflare)
4. **Do NOT** check "Add a README" (we already have one)
5. Click **Create repository**

### Step 2 — Push Files to GitHub

Open Terminal (Mac) or Git Bash (Windows) in the folder with these files:

```bash
git init
git add .
git commit -m "Initial commit — KV portfolio"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/kristina-vishar-portfolio.git
git push -u origin main
```

> Replace `YOUR_USERNAME` with your actual GitHub username.

### Step 3 — Connect to Cloudflare Pages

1. Log in to [dash.cloudflare.com](https://dash.cloudflare.com)
2. In the sidebar, click **Workers & Pages**
3. Click **Create** → **Pages** tab
4. Click **Connect to Git**
5. Authorise GitHub if prompted, then select your repository
6. Configure build settings:

| Setting            | Value  |
|--------------------|--------|
| Production branch  | `main` |
| Build command      | *(leave empty)* |
| Build output directory | `/` |

7. Click **Save and Deploy**

Your site will be live at `https://kristina-vishar-portfolio.pages.dev` within ~1 minute.

### Step 4 — Custom Domain (optional)

1. In Cloudflare Pages → your project → **Custom domains**
2. Click **Set up a custom domain**
3. Enter your domain (e.g. `kristinavishar.com`)
4. Follow DNS instructions — Cloudflare handles SSL automatically

---

## Alternative: Direct Upload (no GitHub needed)

1. Go to [dash.cloudflare.com](https://dash.cloudflare.com) → **Workers & Pages**
2. Click **Create** → **Pages** → **Upload assets**
3. Name your project
4. Drag and drop the entire site folder (or ZIP)
5. Click **Deploy site**

---

## Updating Content

### Replace FAQ / Testimonials placeholder text:
Open `index.html`, find `<!-- ═══ FAQ ═══ -->` and `<!-- ═══ TESTIMONIALS ═══ -->` sections, and edit the text directly.

### Add/replace portfolio images:
1. Put new images in `images/` folder
2. In `index.html`, update the `<img src="images/NewImage.JPG">` paths
3. Commit and push — Cloudflare auto-deploys

### Change booking link:
Search for `https://shorturl.at/YuHjV` in `index.html` and replace all instances.

---

## File Structure

```
/
├── index.html          ← Main site file (all code in one file)
├── README.md           ← This file
└── images/
    ├── Hero.PNG        ← Hero background
    ├── Me_cosplay_1-4.JPG  ← About section photos
    └── Portfolio1-16.JPG   ← Portfolio gallery
```
