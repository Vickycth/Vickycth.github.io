# Vickycth.github.io

Personal academic website for Tianhui Cai, PhD student at UCLA.

Live site (after deploy): **https://vickycth.github.io**

---

## How to deploy this to GitHub Pages

GitHub Pages will automatically serve a website from a repo named `<username>.github.io`. No build step is needed — just push the files.

### Step 1 — Create the GitHub repo

1. Go to https://github.com/new
2. Repository name: **`Vickycth.github.io`** (it must match your GitHub username exactly, case-insensitive)
3. Set it to **Public**
4. Do **not** initialize with README, .gitignore, or license (you already have files)
5. Click **Create repository**

### Step 2 — Push the files

From your terminal, inside this folder:

```bash
git init
git add .
git commit -m "Initial commit: personal website"
git branch -M main
git remote add origin https://github.com/Vickycth/Vickycth.github.io.git
git push -u origin main
```

### Step 3 — Wait & visit your site

Within 1–2 minutes, your site will be live at:

**https://vickycth.github.io**

If it doesn't show up:
- Go to your repo → **Settings** → **Pages**
- Under **Source**, select branch `main` and folder `/ (root)`, then click **Save**

---

## File structure

```
vickycth.github.io/
├── index.html        # Main page (About, Education, Publications, Contact)
├── style.css         # Styling
├── images/
│   └── profile.jpg   # Profile photo placeholder — replace with your real photo
├── files/            # Optional folder for hosting your CV PDF
│   └── (add Tianhui_CV.pdf here)
└── README.md         # This file
```

---

## How to customize

### Replace the profile photo
Replace `images/profile.jpg` with your own photo. Square images work best (e.g., 600×600 px).

### Add your CV
Drop your CV PDF into the `files/` folder named `Tianhui_CV.pdf`. The "CV" link in the sidebar will then work.

### Update the bio / education / publications
Open `index.html` in any text editor (VS Code, Sublime, etc.) and edit the content directly. Each section is clearly commented:
- `<section id="about">` — the About paragraph
- `<section id="education">` — education timeline
- `<section id="publications">` — publication list
- `<section id="contact">` — contact info

### Update social links
In `index.html`, find the `<ul class="social-links">` block and replace the placeholder URLs with your actual Google Scholar / LinkedIn profile links.

### To make changes after deploying
```bash
git add .
git commit -m "Update: <describe your change>"
git push
```
Changes appear on the live site within ~1 minute.

---

## Custom domain (optional)

If you later buy a custom domain (e.g., `tianhuicai.com`), you can use it for free by:
1. Adding a `CNAME` file to the repo with the domain name
2. Configuring DNS records in your domain registrar
3. Enabling the custom domain in GitHub repo Settings → Pages

---

Built with plain HTML & CSS. No build tools, no dependencies, no Jekyll — just push and go.
