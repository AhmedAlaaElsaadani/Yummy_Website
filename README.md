# 🍽️ Yummy — Recipe & Meal Explorer

A responsive recipe-discovery website built with **vanilla HTML, CSS, JavaScript & jQuery**. Search for meals, browse by category, cuisine, or ingredient, and open rich detail pages with instructions, ingredients, and video tutorials — all powered by the free [TheMealDB](https://www.themealdb.com/) API.

<p align="left">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" />
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript&logoColor=black" />
  <img alt="jQuery" src="https://img.shields.io/badge/jQuery-3.6-0769AD?logo=jquery&logoColor=white" />
  <img alt="Bootstrap" src="https://img.shields.io/badge/Bootstrap-5-7952B3?logo=bootstrap&logoColor=white" />
</p>

> 🧠 **100% human-written.** This project was designed and coded entirely by hand — **no AI tools or code generators were used** in its development.

---

## 📑 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Screenshots](#-screenshots)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [API](#-api)
- [Author](#-author)

---

## ✨ Features

- 🔍 **Search by name** — find meals by typing their name (validated for letters).
- 🔤 **Search by first letter** — list meals that start with a single letter.
- 🗂️ **Browse categories** — explore all meal categories with thumbnails and descriptions, then drill into each.
- 🌍 **Browse by area / cuisine** — discover meals by country (Italian, Indian, American, …).
- 🥕 **Browse by ingredient** — pick from a list of ingredients and see matching meals.
- 📄 **Meal details** — full cooking instructions, ingredient list with measurements, tags, plus links to the **YouTube tutorial** and **source recipe**.
- 📝 **Contact form** — with full client-side validation (name, email, Egyptian phone format, age, and strong password rules).
- 🌗 **Dark / light mode** — toggle the theme on the fly.
- 📱 **Animated side navigation** — a sliding hamburger menu and fully responsive layout.
- ⏳ **Loading indicator** — spinner feedback while data is fetched.

---

## 🧰 Tech Stack

| Area | Technology |
|------|-----------|
| Markup & styling | HTML5, CSS3, Bootstrap 5 |
| Logic | Vanilla JavaScript (ES6) + jQuery 3.6 |
| Icons | Font Awesome |
| Data | [TheMealDB](https://www.themealdb.com/) public API |
| Build tooling | None — pure static site |

---

## 🖼️ Screenshots

> _Add your screenshots here, e.g._
>
> | Search | Categories | Meal Details |
> |--------|------------|--------------|
> | ![Search](docs/search.png) | ![Categories](docs/categories.png) | ![Details](docs/details.png) |

---

## 🚀 Getting Started

No build step or installation is required — it's a static site.

```bash
# 1. Clone the repository
git clone https://github.com/AhmedAlaaElsaadani/Yummy_Website.git

# 2. Open the folder
cd Yummy_Website
```

Then either:

- **Open `index.html`** directly in your browser, **or**
- Serve it with a local server (recommended, e.g. the VS Code *Live Server* extension):

  ```bash
  # Python
  python -m http.server 8000
  # or Node
  npx http-server
  ```

  Then visit [http://localhost:8000](http://localhost:8000).

---

## 📂 Project Structure

```
Yummy/
├── index.html          # Single-page app markup
├── js/
│   ├── app.js          # All application logic (search, fetch, render, validation)
│   ├── jquery-3.6.1.js
│   └── bootstrap.bundle.min.js
├── Css/
│   ├── style.css       # Custom styles & animations
│   ├── bootstrap.min.css
│   └── all.css         # Font Awesome
├── Images/             # Logo & theme backgrounds
└── webfonts/           # Font Awesome web fonts
```

---

## 🔌 API

All meal data comes from **[TheMealDB](https://www.themealdb.com/)** (no API key required):

```
https://www.themealdb.com/api/json/v1/1/
```

| Purpose | Endpoint |
|---------|----------|
| Search by name | `search.php?s={name}` |
| Search by letter | `search.php?f={letter}` |
| All categories | `categories.php` |
| All areas | `list.php?a=list` |
| All ingredients | `list.php?i=list` |
| Filter by category / area / ingredient | `filter.php?c=` / `?a=` / `?i=` |
| Meal details by id | `lookup.php?i={id}` |

---

## 👤 Author

**Ahmed Alaa Elsaadani**

- GitHub: [@AhmedAlaaElsaadani](https://github.com/AhmedAlaaElsaadani)

---

> ⭐ If you find this project helpful, consider giving it a star on GitHub!
