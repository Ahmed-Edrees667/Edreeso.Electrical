# Edreeso Electrical Engineering Website

**Ahmed Edrees Mohammed** — Senior Electrical Engineer

## 📁 File Structure

```
edreeso-electrical/
├── index.html        ← Main website (public)
├── admin.html        ← Admin panel (password protected)
├── data.json         ← ALL website content — edit this to update the site
├── profile.jpg       ← Your profile photo (replace with your image)
└── README.md         ← This file
```

---

## 🚀 Deploying to GitHub Pages

### First Time Setup

1. Create a new **GitHub repository** (e.g., `edreeso-electrical`)
2. Upload all files: `index.html`, `admin.html`, `data.json`, `profile.jpg`, `README.md`
3. Go to **Settings → Pages**
4. Under **Source**, select `main` branch → `/root` folder
5. Click **Save**
6. Your site will be live at: `https://YOUR_USERNAME.github.io/edreeso-electrical/`

### Protecting the Site (Only You Can Edit)

GitHub Pages serves static files publicly (read-only for visitors).  
Your site content is controlled entirely via `data.json` — only someone with your GitHub account login can change the files.

To fully protect your admin panel:
- **Never share your GitHub password**
- The admin panel at `admin.html` is protected by a local password
- Default password: `Edreeso@2026` — **change this immediately** in the admin panel

---

## ✏️ How to Update the Site

### Method 1 — Admin Panel (Easiest)
1. Open `https://YOUR_SITE/admin.html`
2. Enter your admin password
3. Add/edit/delete topics, categories, or sections
4. Go to **Import/Export** tab → click **Download data.json**
5. Upload the new `data.json` to your GitHub repository

### Method 2 — Edit data.json Directly
1. Open `data.json` in any text editor
2. Make your changes (add topics, new categories, edit descriptions)
3. Upload the updated file to GitHub

### Adding a New Topic
In `data.json`, find the section and category, then add to the `topics` array:
```json
"topics": [
  "Existing Topic",
  "Your New Topic Here"
]
```

### Adding a Topic with Images
Topics with images are explained automatically by the AI engine.  
To add custom images to a topic explanation, you can include image URLs in the topic name or add them via the raw JSON editor in the admin panel.

### Adding a New Section
In the admin panel → **Sections** tab → click **＋ New Section**  
Or copy an existing section block in `data.json` and modify it.

---

## 🔒 Security Notes

- The website is **read-only** for all visitors
- Only the GitHub account owner can push changes to the repository
- The admin panel is protected by a local browser password
- To change the admin password: open `admin.html` → Login → **Import/Export** tab → Change Password section
- **Important**: The admin password is stored locally in your browser. If you use a different browser/device, it resets to the default: `Edreeso@2026`

---

## 🔧 Technical Details

- **No backend required** — pure static HTML/CSS/JS
- Content loaded dynamically from `data.json`
- Topic explanations powered by **Claude AI API** (Anthropic)
- Compatible with GitHub Pages, Netlify, or any static host
- Fully responsive (mobile/tablet/desktop)

---

## 📞 Contact

Ahmed Edrees Mohammed  
📧 Ahmed.edrees.mohammed@gmail.com  
📞 +20 111 134 8097  
📍 Sohag, Egypt
