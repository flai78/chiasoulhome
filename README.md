# Chia Soul Home

A static website for **Chia Soul Home** — a charming stone villa in Chia, south Sardinia.

## 🌐 Live Site

Once deployed, the site will be available at:  
`https://<your-github-username>.github.io/chiasoulhome/`

---

## 🚀 Deploy to GitHub Pages (step by step)

### 1. Initialise a git repository (if not done already)
```bash
cd /Users/filippolai/Documents/chia/chiasoulhome
git init
git add .
git commit -m "Initial commit — Chia Soul Home website"
```

### 2. Create a repository on GitHub
- Go to [github.com/new](https://github.com/new)
- Name it **`chiasoulhome`** (or any name you like)
- Leave it **Public** (required for free GitHub Pages)
- Do **not** initialise with a README

### 3. Push your code
```bash
git remote add origin https://github.com/<your-username>/chiasoulhome.git
git branch -M main
git push -u origin main
```

### 4. Enable GitHub Pages
- In your repository, go to **Settings → Pages**
- Under *Source*, select **Deploy from a branch**
- Choose branch **`main`** / folder **`/ (root)`**
- Click **Save**

Your site will be live in ~1 minute at:  
`https://<your-username>.github.io/chiasoulhome/`

---

## 📬 Set up the contact form

The contact form uses [Formspree](https://formspree.io) — free up to 50 submissions/month.

1. Create a free account at [formspree.io](https://formspree.io)
2. Create a new form — you'll receive a form ID like `xpzgkrqv`
3. In `index.html`, replace `YOUR_FORM_ID` in:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" ...>
   ```
   with your actual ID, e.g. `https://formspree.io/f/xpzgkrqv`

---

## 📁 Project Structure

```
chiasoulhome/
├── index.html        ← main page
├── css/
│   └── style.css     ← all styles
├── img/              ← all property photos
└── README.md
```

---

## ✏️ Customisation tips

| What to change | Where |
|---|---|
| Owner contact email | Formspree form settings |
| Property description text | `index.html` — `#about` section |
| Number of guests / bedrooms | `index.html` — `.about-stats` |
| Map coordinates | `index.html` — `<iframe>` `src` URL |
| Colour palette | `css/style.css` — `:root` variables |
