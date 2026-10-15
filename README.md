# Boronia Arts — Website 🎨

A friendly, single-page website for **Boronia Arts** — drawing & painting classes for children aged 4–14.

Built as **one self-contained `index.html` file** (HTML + CSS + JavaScript in a single file, no frameworks, no build tools). Perfect for free hosting on **GitHub Pages**.

---

## What's in this folder

| File | What it is |
|---|---|
| `index.html` | The entire website — every section, style and script in one file |
| `DEPLOYMENT_GUIDE.md` | **Start here if you're a beginner** — step-by-step instructions to put this site online for free |
| `.nojekyll` | A tiny (empty) file that tells GitHub Pages "serve exactly these files" — don't delete it |
| `README.md` | This file |

## Try it on your own computer first

1. Find `index.html` in this folder.
2. Double-click it (it opens in your browser — Chrome, Edge, whatever you have).
3. That's it. That's the whole website.

## Edit it with any text editor

Open `index.html` in **Notepad** (Windows) / **TextEdit** (Mac) / VS Code and search for the word **`EDIT`** (press `Ctrl + F`). Every place you should customise is marked with a `✏️ EDIT` comment — your address, phone, WhatsApp number, fees, timings, teacher's name, and the sample gallery/testimonials.

The form buttons (WhatsApp / email) start working as soon as you fill in two lines in the `SITE` settings near the bottom of the file:

```js
const SITE = {
  whatsappNumber: "919876543210",   // ← your WhatsApp number, digits only
  email: "hello@boroniaarts.com",   // ← your email
};
```

## Put it online (free)

Full beginner instructions with every click explained: **[DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md)**.

Short version — create a free GitHub account, upload these files to a new repository, then turn on **Settings → Pages**. Your site goes live at `https://YOUR-USERNAME.github.io/boronia-arts/` in about a minute.

## License / ownership

All content, artwork and the Boronia Arts name belong to you. Free to host, edit and share.
