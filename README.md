# Art With Heart Website

A Girl Scout Gold Award Project by Safiya - providing accessible art and mental health resources for refugee children.

---

## 🚀 Setup Instructions

### Step 1: Download Images from the Original Site

You need to download these images from the Webnode site and place them in the `images/` folder:

| Save As | Original URL |
|---------|--------------|
| `logo.png` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000035-2458724589/Green%20Orange%20and%20Blue%20Cute%20Kindergarten%20Logo-2.jpeg |
| `safiya-books.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000042-c0d54c0d56/IMG_7871.jpeg |
| `gold-award-logo.png` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000070-421cf421d0/Gold%20Logo.png |
| `radiant-hands.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000058-7f5d97f5dc/IMG_8896.jpeg |
| `back-to-school.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000060-cc211cc212/0AFB3959-F1EE-4AD9-B7D3-B8E27384140D.jpeg |
| `global-refuge.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000056-1dd961dd98/IMG_9168.jpeg |
| `girl-scout-events.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000046-bdf93bdf95/IMG_9210.jpeg |
| `patch-program.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000048-c4d76c4d78/IMG_7653.jpeg |
| `presentations.jpg` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000044-3a64a3a64c/Troop%2030124-2025.12.02_%20Art%20with%20Heart%20%40SU-74223306865.jpeg |
| `collaborative-art.png` | https://d56486db30.cbaul-cdnwnd.com/e8241c03b33c73ec15ac427b90b27ce1/200000098-b7faab7fab/Screenshot%202026-01-16%20at%204.04.39%E2%80%AFPM.png |

**To download:** Right-click each link → "Save link as..." → Save with the filename in the first column.

---

### Step 2: Add Activity Book PDFs

Place your activity book PDF files in the `files/` folder:
- `files/activity-book-english.pdf`
- `files/activity-book-spanish.pdf`
- `files/activity-book-arabic.pdf`

---

### Step 3: Set Up Contact Form (Free)

The contact form uses [Formspree](https://formspree.io/) (free tier allows 50 submissions/month):

1. Go to https://formspree.io/ and create a free account
2. Create a new form and copy your form endpoint (looks like `https://formspree.io/f/xyzabc123`)
3. Open `contact.html` and replace `YOUR_FORMSPREE_ID` with your form ID

---

### Step 4: Upload to GitHub

1. Create a new repository on GitHub (e.g., `art-with-heart`)
2. Upload all files from this folder to the repository
3. Go to **Settings → Pages**
4. Under "Source", select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click Save

Your site will be live at: `https://yourusername.github.io/art-with-heart/`

---

### Step 5: Connect Your Custom Domain (artwithheartproject.com)

#### In GitHub:
1. Go to your repository **Settings → Pages**
2. Under "Custom domain", enter: `artwithheartproject.com`
3. Click Save
4. Check "Enforce HTTPS" (may take a few minutes to become available)

#### In Namecheap:
1. Log into Namecheap → **Domain List** → click **Manage** next to artwithheartproject.com
2. Go to **Advanced DNS**
3. Delete any existing A records or CNAME records for @ or www
4. Add these **A Records** (Host: `@`):
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
5. Add a **CNAME Record**:
   - Host: `www`
   - Value: `yourusername.github.io.` (replace with your GitHub username, include the trailing dot)
6. Wait 10-30 minutes for DNS to propagate

---

## 📁 File Structure

```
art-with-heart/
├── index.html              # Home page
├── activity-books.html     # Activity books download page
├── refugee-experience.html # About the refugee experience
├── art-mental-health.html  # Art therapy information
├── contact.html            # Contact form
├── style.css               # Main stylesheet
├── images/                 # All images go here
│   ├── logo.png
│   ├── safiya-books.jpg
│   └── ... (other images)
├── files/                  # PDF activity books go here
│   ├── activity-book-english.pdf
│   ├── activity-book-spanish.pdf
│   └── activity-book-arabic.pdf
└── README.md               # This file
```

---

## ✏️ Making Changes

To edit the website content, simply edit the HTML files. The site uses plain HTML/CSS with no build process required.

- **Change text:** Edit the HTML files directly
- **Change colors:** Edit the CSS variables at the top of `style.css`
- **Add pages:** Create new HTML files following the same structure

---

## Need Help?

If you run into any issues, feel free to reach out!
