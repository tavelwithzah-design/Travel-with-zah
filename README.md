# Travel With Zaaheer — Website

A beautiful, image-first travel website. Elegant. Royal. Simple.

---

## How to Go Live (5 Steps)

### 1. Upload to GitHub
Create a new GitHub repository and push all these files to it.

### 2. Deploy to Netlify
- Go to netlify.com → "Add new site" → "Import from GitHub"
- Select your repository
- Click **Deploy** (no build settings needed — it's just HTML)

### 3. Enable Netlify Identity
- In your Netlify dashboard → **Integrations** → search for **Identity**
- Enable it
- Under Identity settings → **Registration** → set to **Invite only**
- Under Identity settings → **Git Gateway** → Enable it

### 4. Invite Yourself as Admin
- In Netlify Identity → click **Invite users**
- Enter your email address
- Accept the invite email and set your password

### 5. Access the CMS
- Go to **yoursite.com/admin**
- Log in with your email + password
- You can now add posts, upload photos, and publish stories!

---

## File Structure

```
/
├── index.html          ← Homepage
├── journal.html        ← All blog posts listing
├── post.html           ← Sample story page (template)
├── css/
│   └── style.css       ← All styles
├── admin/
│   ├── index.html      ← CMS admin interface
│   └── config.yml      ← CMS configuration
├── images/
│   └── uploads/        ← Your uploaded images go here
├── _posts/             ← Blog post files (created by CMS)
└── netlify.toml        ← Netlify config
```

---

## Replacing Placeholder Images

The site currently uses Unsplash placeholder images.
Replace them with your own travel photos by editing the `src=""` attributes in the HTML files.

**Best image sizes:**
- Hero images: 1800px wide, landscape orientation
- Gallery cards: 1200px wide
- Blog post inline images: 1400px wide

---

## Adding Your Own Travel Photos & Stories

Use the CMS at `/admin` to:
- Add new journal posts
- Upload your own travel photography
- Write story content with the rich text editor
- Publish when ready

---

## Customisation

- **Colors & fonts**: Edit `css/style.css` (look for the `:root` variables at the top)
- **Homepage placeholder cards**: Edit `index.html` grid section
- **Your bio/about text**: Add a new page or edit the intro text in `index.html`
