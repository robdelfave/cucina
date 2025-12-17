# Cucina Website

GitHub Pages site for Cucina recipe organizer app.

## Setup Instructions

### 1. Create New GitHub Repository

1. Go to https://github.com/new
2. Repository name: `cucina-app` (or any name you prefer)
3. Description: `Website and legal docs for Cucina recipe app`
4. Make it **Public**
5. ✅ Add a README file
6. Click **Create repository**

### 2. Upload Files

1. In your new repository, click **Add file** → **Upload files**
2. Upload these three files:
   - `index.html`
   - `privacy.html`
   - `terms.html`
3. Commit message: "Add website and legal pages"
4. Click **Commit changes**

### 3. Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll down to **Pages** (in left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Under "Branch", select **main** (or **master**)
5. Select folder: **/ (root)**
6. Click **Save**

### 4. Wait for Deployment

- GitHub will build your site (takes 1-2 minutes)
- You'll see a green checkmark when ready
- Your site will be live at: `https://yourusername.github.io/cucina-app/`

### 5. Get Your URLs

Once deployed, your pages will be available at:

- **Homepage:** `https://yourusername.github.io/cucina-app/`
- **Privacy Policy:** `https://yourusername.github.io/cucina-app/privacy.html`
- **Terms of Service:** `https://yourusername.github.io/cucina-app/terms.html`

### 6. Update Cucina App

Replace URLs in `SettingsView.swift`:

```swift
// Legal Section
Link(destination: URL(string: "https://yourusername.github.io/cucina-app/privacy.html")!) {
    Label("Privacy Policy", systemImage: "hand.raised")
}

Link(destination: URL(string: "https://yourusername.github.io/cucina-app/terms.html")!) {
    Label("Terms of Service", systemImage: "doc.text")
}
```

### 7. Update Contact Email

Update `your-email@example.com` in all three HTML files:

- `index.html` (line ~94 and ~106)
- `privacy.html` (line ~142)
- `terms.html` (line ~173)

Search and replace:
- Find: `your-email@example.com`
- Replace with: `your-actual-email@domain.com`

### 8. Test Your Site

1. Visit your GitHub Pages URL
2. Click through all pages
3. Test the email links
4. View on mobile to ensure responsive design

---

## Customization

### Update Content

To update any page:
1. Edit the HTML file in GitHub (click pencil icon)
2. Make your changes
3. Commit changes
4. Site updates automatically in 1-2 minutes

### Change Colors

In each HTML file, find the `<style>` section and update:
- Primary color: `#007AFF` (iOS blue)
- Secondary color: `#5856D6` (iOS purple)
- Background gradient: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`

### Add Custom Domain (Optional)

1. Buy a domain (e.g., `cucina-app.com`)
2. In repository Settings → Pages → Custom domain
3. Enter your domain
4. Update DNS settings with your domain registrar

---

## Important Notes

- **Public Repository:** These pages are publicly accessible
- **SSL Enabled:** GitHub Pages provides free HTTPS
- **Fast Loading:** Static HTML loads instantly
- **No Hosting Costs:** Completely free with GitHub
- **Version Control:** All changes are tracked in Git

---

## App Store Connect

When submitting to App Store, use these URLs:

- **Privacy Policy URL:** `https://yourusername.github.io/cucina-app/privacy.html`
- **Support URL:** `https://yourusername.github.io/cucina-app/` (optional)
- **Marketing URL:** `https://yourusername.github.io/cucina-app/` (optional)

---

## File Structure

```
cucina-app/
├── index.html          # Homepage
├── privacy.html        # Privacy Policy (required for App Store)
├── terms.html          # Terms of Service (required for App Store)
└── README.md           # This file
```

---

## Maintenance

### Update Last Modified Date

When updating privacy.html or terms.html, change:
```html
<p class="last-updated">Last updated: December 17, 2024</p>
```

### Legal Changes

If you make significant changes to privacy or terms:
1. Update the "Last updated" date
2. Notify existing users (via app update notes)
3. Consider adding a changelog section

---

## Questions?

- GitHub Pages Docs: https://docs.github.com/pages
- HTML Validation: https://validator.w3.org/
- Mobile Testing: Use Chrome DevTools → Toggle Device Toolbar

---

Built with ❤️ by Robert Delfave
