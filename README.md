# Pawfect Care — Web App

A lightweight, mobile-first web app for discovering trusted pet caregivers and showcasing caregiver profiles.

## ✨ Features

- **Hero + value prop**: quick intro with CTA.

- **Care mode toggle**: switch between “I need care” and “I’m a caregiver”.

- **Pet type selector**: Dog / Cat / Other.

- **Caregiver cards**: avatar, distance, rating, services/tags, call-to-action.

- **Verification steps**: clear onboarding path for new caregivers.

- **Responsive layout**: looks great on phone and desktop.

- **Vanilla stack**: simple HTML + CSS (no build tools required).

---
## 🧱 Tech Stack

- **HTML5** for structure

- **CSS3** for styling (mobile-first, utility-like helpers)

- (Optional) A tiny bit of vanilla JS if you add interactivity later

----

## 📁 Project Structure

web/

├─ index.html         # Main page markup

├─ style.css          # Styles (colors, layout, cards, utilities)

└─ assets/            # (Optional) images, icons, favicons

----
## 🚀 Getting Started

### **Option A — Open directly**

1. Download the project.

2. Double-click `index.html` to open it in your browser.

### **Option B — Run a tiny local server (recommended)**

This avoids CORS issues with images/fonts on some browsers.
```bash
# Python 3
python -m http.server 8080
# open http://localhost:8080 in your browser
```
## 🎨 Customization

- **Brand colors**: update CSS variables or color classes in `style.css`.

- **Copy & headings**: edit the hero text, section titles, and card content in index.html.

- **Caregiver cards**: duplicate a card block and replace:

      - `name`, `distance`, `rating`, `services/tags`

      - `image` and `avatar` URLs

- **Sections**: comment out or duplicate sections to fit your needs.

  ---

## ♿ Accessibility (Quick Checklist)

- Use **semantic element** (`<header>`, `<main>`, `<section>`, `<footer>`).

- Ensure **color contrast** (check primary/secondary on light backgrounds).

- Provide **alt text** for all images/avatars.

- Keep **button labels** descriptive (e.g., “View Profile”).

- Maintain **focus states** for clickable elements.

---

## 🔍 SEO

- Set a descriptive `<title>` and `<meta name="description">` in `index.html`.

- Add Open Graph tags for better sharing:
```bash
<meta property="og:title" content="Pawfect Care – Find Trusted Pet Caregivers" />
<meta property="og:description" content="Discover vetted caregivers for dogs, cats, and more." />
<meta property="og:image" content="assets/cover.jpg" />
<meta property="og:type" content="website" />
```
 - Include a **favicon** in `/assets`.
----

## 🌐 Deployment

- **GitHub Pages**: push to `main`, enable Pages → set root to `/` (or `/docs` if you move files).

- **Netlify / Vercel**: drag-and-drop the folder or connect your repo; use default static site settings.

---

## 🔌 Hooking up a backend 

When you’re ready to go dynamic:

- Replace hardcoded caregiver cards with data fetched from an API.  
- Add a simple script:

```html
<script>
  async function loadCaregivers() {
    const res = await fetch('/api/caregivers'); // your endpoint
    const items = await res.json();
    // render into a container with template literals
  }
  // loadCaregivers();
</script> ```

- Consider adding search/filter inputs and wiring them to the API.
---
🧭 Roadmap

 - Real data (caregivers, ratings, tags) from API

 - Search & filters (distance, services, price)

 - Auth (owner/caregiver)

 - Booking flow + messaging

 - PWA (offline, home-screen icon)

 - i18n (EN/FA toggle)
---

## 🤝 Contributing

1. Fork the repository

2. Create a feature branch: `git checkout -b feat/your-feature`

3. Commit changes: `git commit -m "feat: add your feature"`

4. Push: `git push origin feat/your-feature`

5. Open a Pull Request

----
## 📬 Contact
For questions or collaboration opportunities:

**📧 Email**: ali.razi9292@gmail.com

**🔗 LinkedIn**: linkedin.com/in/alirazi1992
