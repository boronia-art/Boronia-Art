# 🚀 Boronia Arts — Deployment Handover Guide

*Written for a complete beginner. No coding experience needed. Everything is free.*

---

## What you are deploying (60-second explainer)

Your website is a **single file** called `index.html`. When someone visits your web address, a free service called **GitHub Pages** hands that file to their browser, and the page appears. There is:

- ✅ **No server to rent** — GitHub hosts it free, forever, with no ads
- ✅ **No database, no logins, no monthly bills**
- ✅ **Nothing to break** — the file either works (it does) or you re-upload it

The only thing you'll ever do again is *edit the file and re-upload it* — that's how you change fees, photos, anything.

> ⏱ **Total time: about 20 minutes, once.**

---

## Part 0 — What you need before you start

1. The files you received: `index.html`, `README.md`, `DEPLOYMENT_GUIDE.md` (this file), `.nojekyll`.
   *(If you have the `boronia-arts-website.zip`, unzip it first — right-click → Extract All.)*
2. A computer with a normal browser.
3. Your **real details** handy (you'll paste them in Step 1): address, phone, WhatsApp number, email, fees, batch timings.

---

## Part 1 — Personalise the site (do this BEFORE going live)

You don't want `[Add your address]` showing on a live website!

1. **Open `index.html` in a text editor.**
   - Windows: right-click the file → *Open with* → **Notepad**.
   - Mac: right-click → *Open With* → **TextEdit** (or install the free **VS Code** for a nicer experience).
2. **Press `Ctrl + F`** (Mac: `Cmd + F`) and search for the word: `EDIT`
3. Every match is a spot to personalise. Fill in this checklist:

| # | Search for | What to replace it with |
|---|---|---|
| 1 | `[Teacher's name]` | The teacher's / founder's name (About section) |
| 2 | `[Add your street address]` | Your studio address (Contact section + FAQ) |
| 3 | `[+91 XXXXX XXXXX]` | Your phone number |
| 4 | `[hello@yourstudio.com]` | Your email |
| 5 | `[Add your batch timings]` | Your class hours |
| 6 | `[Days]`, `[Time]`, `[fee]` | Real schedule & fees (Schedule table) |
| 7 | `whatsappNumber: ""` | `whatsappNumber: "919876543210"` — your WhatsApp in international format, digits only (this makes the form + green chat bubble work) |
| 8 | `email: ""` | `email: "hello@boroniaarts.com"` — makes the "email instead" button work |
| 9 | `Instagram (add link)` / `Facebook (add link)` | Your real page URLs in the footer `href="#"` |
| 10 | Sample gallery pieces | Optional: replace the 6 sample drawings with photos of real student art (see Part 4) |
| 11 | Testimonials marked `SAMPLE` | Real parent quotes (with their permission) + the sample stats in the About section |
| 12 | `Write your story here` | 2–3 lines about the teacher's background |

4. **Save the file** (`Ctrl + S`) and double-click it to preview in your browser.

> 💡 The website's **form doesn't need any server**. Tapping "Send on WhatsApp" opens WhatsApp with the enquiry pre-typed. It works the moment you fill in line 7 above.

---

## Part 2 — Publish to the internet (GitHub Pages)

### Step 1 — Create a free GitHub account (2 min)

1. Go to **[github.com](https://github.com)** and click **Sign up**.
2. Enter an email, create a password, pick a username.
   - Tip: your username becomes part of your web address — something like `boronia-arts` is ideal.
3. Verify your email when GitHub asks.

### Step 2 — Create a repository ("a folder in the cloud") (2 min)

1. Log in to GitHub. Click the **`+`** at the top-right → **New repository**.
2. **Repository name:** `boronia-arts` (exactly — lowercase, with the hyphen).
3. Visibility: **Public** (required for the free hosting).
4. Click **Create repository**.
5. You'll land on a page saying "Quick setup" — **don't run any commands**. Leave this tab open.

### Step 3 — Upload the website files (3 min)

1. On that same page, find the link **"uploading an existing file"** and click it.
2. **Drag all your files** (`index.html`, `README.md`, `DEPLOYMENT_GUIDE.md`, `.nojekyll`) into the big upload box.
   - Windows: make sure hidden files are visible so you can see `.nojekyll`. Can't see it? Skip it — or create it later (Step 4b below).
3. Click **Commit changes** (GitHub's word for "Save/upload").
4. You should now see `index.html` listed in your repository. 🎉

### Step 4 — Turn on the website (2 min)

1. In your repository, click **Settings** (top menu) → **Pages** (in the left sidebar).
2. Under **"Build and deployment"**:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` — Folder: `/(root)`
3. Click **Save**.
4. Wait **1–2 minutes**, then refresh the page. A green box appears:

   > **Your site is live at `https://YOUR-USERNAME.github.io/boronia-arts/`**

5. **Click that link.** Your website is on the internet. Share it with everyone. 🥳

> **4b — If something looks wrong on the live site** (e.g. styles seem ignored): go back to the repository main page → **Add file → Create new file** → name it exactly `.nojekyll` (the leading dot matters) → leave it empty → Commit. This tells GitHub to serve files as-is.

### Step 5 — Set up the WhatsApp & email buttons (2 min)

1. Open `index.html` (from your computer).
2. Find the `SITE` settings near the bottom and fill in your **WhatsApp number** and **email** (Part 1, items 7–8).
3. Save, then upload the new version of `index.html`:
   - GitHub → your repo → click `index.html` → the **pencil icon** ✏️ (top-right of the file view).
   - Or: **Add file → Upload files** → drag the new `index.html` → **Commit changes**.
4. Wait ~1 minute — GitHub re-publishes automatically after every upload.

---

## Part 3 — Everyday edits (how you update the site later)

**Any time you want to change something — fees, a photo, a word:**

1. Open `index.html` in Notepad, make your change, save.
2. GitHub → your repo → **Add file → Upload files** → drop in `index.html` → **Commit changes** (this replaces the old version).
3. Refresh your live link after ~1 minute.

That's the whole workflow: **edit → upload → commit.** No developer needed.

> 💡 If the live site still shows the old version: press **`Ctrl + F5`** (hard refresh) in your browser — it's just cached.

---

## Part 4 — Replacing the gallery with real student artwork (optional but lovely)

The gallery currently shows 6 built-in sample drawings so the site looks complete. To use real photos:

1. Put the photo files (e.g. `art1.jpg`, ideally landscape-ish, under ~500 KB each) **in the same folder** as `index.html`.
2. In `index.html`, find the `<figure class="frame reveal" ...>` blocks in the GALLERY section.
3. Replace the whole `<svg>…</svg>` inside a figure with:
   ```html
   <img src="art1.jpg" alt="Watercolour painting by a student, age 8">
   ```
4. Keep the `<figcaption>` — edit the title/medium/age text.
5. Upload the photos **and** `index.html` to GitHub together (Step 3 above).

**Before publishing photos of children:** use artwork-only shots where possible; if a child's face is visible, get the parents' written permission first.

---

## Part 5 — Troubleshooting

| Problem | Fix |
|---|---|
| Live link shows **404** | Wait 2 minutes and refresh. Check Settings → Pages: Branch must be `main`, folder `/(root)`. |
| Site loads but **looks like plain text / unstyled** | Create the `.nojekyll` file (Step 4b). Then hard-refresh (`Ctrl + F5`). |
| **Changes don't appear** | It's browser cache — `Ctrl + F5`, or wait a minute for GitHub to rebuild. |
| **WhatsApp button says "not set up"** | You haven't filled `whatsappNumber` in the `SITE` settings (Part 1, item 7). Digits only, with country code (e.g. `919876543210`). |
| **Form doesn't send an email** | The email button opens the visitor's own mail app — it needs `email: "…"` set in `SITE`. Consider WhatsApp as the primary channel. |
| **Wrong spelling / price live** | Edit → upload → commit (Part 3). Fixes take ~1 minute to go live. |

---

## Part 6 — Optional upgrades (only when you're ready)

- **Your own domain** (e.g. `www.boroniaarts.com`, ~₹700–900/year from any registrar): buy it → in GitHub repo **Settings → Pages → Custom domain**, type the domain and follow GitHub's DNS instructions. The guide at docs.github.com ("Configuring a custom domain for GitHub Pages") walks you through it.
- **A Google Maps embed:** in the Contact section, paste Google's "embed a map" `<iframe>` snippet where you'd like it.
- **Search-engine visibility:** the page already has SEO title/description. After launch, add your link to Google via **Google Search Console** and it will start appearing in search within days/weeks.
- **Other free hosts:** Netlify ([netlify.com/drop](https://app.netlify.com/drop) — literally drag the folder onto the page) or Vercel. GitHub Pages is recommended here because everything stays in one free account you control.

---

## Quick reference card

| Thing | Where |
|---|---|
| Your website files | `index.html` (+ this guide) |
| Live address | `https://YOUR-USERNAME.github.io/boronia-arts/` |
| Publish / update | github.com → your repo → upload → commit |
| Edit anything | Open `index.html`, search `EDIT` |
| Hosting cost | ₹0 |
| Support | [docs.github.com/pages](https://docs.github.com/en/pages) |
