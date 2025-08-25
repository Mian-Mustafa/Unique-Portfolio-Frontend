# Portfolio Website

A clean, responsive personal portfolio built with **HTML**, **CSS**, and **Bootstrap 5**, enhanced with **AOS (Animate On Scroll)** and **Line Awesome** icons.

Use this repo to showcase your services, projects, experience, blog posts, and contact form.

---

## ✨ Demo


* **Screenshot/Preview:**
<img width="1900" height="929" alt="image" src="https://github.com/user-attachments/assets/f21980bf-ed43-4315-a91b-e170727ca14e" />
<img width="1902" height="926" alt="image" src="https://github.com/user-attachments/assets/307b421b-7dcf-4b7f-a5ff-4b36944d2c19" />
<img width="1893" height="931" alt="image" src="https://github.com/user-attachments/assets/73518467-46f1-4e41-98b1-41ba507d73be" />
<img width="1900" height="925" alt="image" src="https://github.com/user-attachments/assets/fc4e0eaf-2b97-468b-b0f5-cc1cce8d0a3e" />
<img width="1899" height="921" alt="image" src="https://github.com/user-attachments/assets/de2ff84a-14dd-4dca-9941-ecbefb11cbc8" />
<img width="1897" height="925" alt="image" src="https://github.com/user-attachments/assets/06a6bf54-5b7e-4bd5-a6e2-71703e8549a4" />
<img width="1907" height="924" alt="image" src="https://github.com/user-attachments/assets/b492a5d4-2147-47fb-82d2-b5055630d494" />
<img width="614" height="910" alt="image" src="https://github.com/user-attachments/assets/dedacb3e-4623-4469-83d3-5253feae566a" />


---

## 🧰 Tech Stack

* **HTML5** & **CSS3**
* **Bootstrap 5** (`bootstrap.min.css`, `bootstrap.bundle.min.js`)
* **AOS** (Animate On Scroll)
* **Line Awesome** icons
* **Google Fonts**: *Bai Jamjuree*

---

## 📁 Project Structure

```
.
├── index.html
├── style.css               # Custom styles
├── main.js                 # AOS configuration & JS hooks
└── assets/
    ├── css/
    │   ├── bootstrap.min.css
    │   ├── aos.css
    │   └── line-awesome.min.css
    ├── js/
    │   ├── bootstrap.bundle.min.js
    │   └── aos.js
    └── images/
        ├── person.png
        ├── sidebar-img.jpg
        ├── project-1.jpg
        ├── project-2.png
        ├── project-3.png
        ├── project-4.png
        ├── blog-post-1.jpg
        ├── blog-post-2.jpg
        └── blog-post-3.jpg
```

> **Note:** Update file paths in `index.html` if you move assets.

---

## 🚀 Getting Started

### 1) Clone the repo

```bash
git clone https://github.com/Mian-Mustafa/Unique-Portfolio-Frontend
cd <https://github.com/Mian-Mustafa/Unique-Portfolio-Frontend>
```

### 2) Open locally

* Option A: Simply open `index.html` in your browser.
* Option B (recommended): Use a local server for correct asset loading

  * VS Code → Install **Live Server** extension → Right‑click `index.html` → **Open with Live Server**.

---

## 🧩 How It’s Built

### HTML (`index.html`)

* **Navbar** (fixed sidebar on large screens)
* Sections: **Home**, **Services**, **Work**, **About**, **Reviews**, **Blogs**, **Contact**
* Uses Bootstrap grid (`container`, `row`, `col-*`) and utility classes
* AOS attributes like `data-aos="fade-up"`, `data-aos-delay="300"` for animations

### CSS (`style.css`)

* Custom theme via CSS variables:

  * `--color-base`, `--color-base2`, `--color-brand`, etc.
* Responsive sidebar at `@media (min-width: 992px)`
* Reusable utilities: `.full-height`, `.shadow-effect`, `.iconbox`, `.card-custom`, `.link-custom`, `.btn-brand`

### JS (`main.js`)

AOS initialization and defaults:

```js
AOS.init();
AOS.init({
  offset: 120,
  delay: 0,
  duration: 1000,
  easing: 'ease',
  once: false,
  mirror: false,
  anchorPlacement: 'top-bottom',
});
```

*Tune these values to speed up/slow down or change trigger behavior.*

---

## 🛠 Customization Guide

### Basic Text & Identity

* **Page title**: update `<title>Ghulam Mustafa</title>` in `index.html`.
* **Hero heading & tagline**: edit the `#home` section.
* **Phone number**: change the `Call: (+92) 324 4269023` link.

### Profile & Images

* Replace `/assets/images/person.png` with your picture (maintain file name or update `src`).
* Update project thumbnails (`project-*.jpg/png`) and blog images (`blog-post-*.jpg`).

### Social Links

Replace `href="#"` with real URLs in the footer:

```html
<div class="social-links">
  <a href="https://github.com/<you>"><i class="lab la-github"></i></a>
  <a href="https://instagram.com/<you>"><i class="lab la-instagram"></i></a>
  <a href="https://facebook.com/<you>"><i class="lab la-facebook"></i></a>
  <a href="https://wa.me/<your-number>"><i class="lab la-whatsapp"></i></a>
  <a href="https://x.com/<you>"><i class="lab la-twitter"></i></a>
</div>
```

### Colors & Theme

Adjust CSS variables in `:root` (inside `style.css`):

```css
:root{
  --color-body: #b6cbce;
  --color-heading: #eef3db;
  --color-base: #033f47;
  --color-base2: #022a30;
  --color-brand: #e0f780;
  --color-brand2: #deff58;
  --sidebar-width: 240px; /* typo fix: was --sidbar-width */
  --font-base: "Bai Jamjuree";
}
```

> **Tip:** Also fix occurrences of `--sidbar-width` → `--sidebar-width` in CSS and where used.

### AOS Effects

You can change per‑element animations using attributes:

```html
<h1 data-aos="flip-up"></h1>
<div data-aos="fade-up" data-aos-delay="300"></div>
```

Full list: [AOS docs](https://michalsnik.github.io/aos/) *(add as a reference in your repo description)*

---

## 🌐 Deployment

### GitHub Pages

1. Push code to `main`.
2. Repo Settings → **Pages** → Source: `Deploy from a branch` → Branch: `main` → `/root`.
3. Wait for build; your site will be available at `https://<username>.github.io/<repo>/`.

### Netlify / Vercel

* Drag‑and‑drop the repo folder to Netlify, or import the Git repo on Vercel.
* Set root directory to repo root; no build step required (static site).

---

## ✅ Accessibility & SEO Quick Wins

* Add `alt` text to all images (`alt="Project thumbnail"`).
* Ensure color contrast meets WCAG AA.
* Add meta description in `<head>`:

  ```html
  <meta name="description" content="UI/UX Designer & Front-end Developer portfolio showcasing services, projects, blog, and contact details.">
  ```
* Use semantic headings (H1 → H2 → H3).

---

## 🔧 Known Issues / Notes

* **Typos** within content (optional to fix):

  * `I,M` → `I’m`, `PAKISTAN ,LHR` → `Lahore, Pakistan`
  * `Inovation` → `Innovation`, `tempelate equiped` → `template equipped`
  * `Studing` → `Studying`, `dababase` → `database`, `Interne` → `Intern`
  * `Whats our Suscribers say` → `What our Subscribers say`
* Consider adding a real contact backend (Formspree, Netlify Forms) if you need email submissions.

---

## 📦 Credits

* **Bootstrap 5** — layout & components
* **AOS** — scroll animations
* **Line Awesome** — icon set
* **Google Fonts** — Bai Jamjuree

---

## 📝 License

This project is open‑sourced under the **MIT License**. Feel free to use and modify for personal or commercial purposes. *(Add a `LICENSE` file to this repo to formalize.)*

---

## 🤝 Contact

**Ghulam Mustafa**
Phone: `(+92) 324‑4269023`
Email: *(add your email)*
LinkedIn: *(add your profile)*

If you use this template, a ⭐ on the repo would be awesome!
