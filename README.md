# ZINIQ — Product Website

> A static marketing website for **ZINIQ** — a dietary supplements brand. The site presents the product range, brand values, ingredient information, and purchase options.

---

## About the Project

This is a multi-page HTML/CSS/JS website built for **ZiNIQ Sp. z o.o.**, a Polish dietary supplements company. The site serves as the primary online presence for the brand, showcasing individual products with detailed ingredient data, dosage information, and purchase guidance.

The site was developed as a custom front-end implementation using Bootstrap 5 as the layout framework, enriched with several third-party UI libraries for sliders, lightboxes, and icon sets.

---

## Pages

| File | Description |
|---|---|
| `index.html` | Homepage — brand introduction, featured products |
| `produkty.html` | Full product listing |
| `produkt.html` | Single product page (Magnez + Witamina B6) |
| `potrzeby-organizmu.html` | Educational section — body's nutritional needs |
| `w-co-wierzymy.html` | Brand values and philosophy |
| `gdzie-kupic.html` | Where to buy — retailer/store information |
| `kontakt.html` | Contact page |

---

## Product Catalogue

Products presented on the site include:

- **Magnez + Witamina B6** — 60 mg magnesium lactate + 1.4 mg Vitamin B6, 50 tablets
- **Magnez + Potas + Witamina B6** — extended electrolyte formula
- **Elektrolity Witaminy + Minerały** — multi-electrolyte supplement
- **Wątroba Cholina + Fosfolipidy** — liver support formula

Each product page includes an ingredients table with % Reference Daily Values (RDV), dosage recommendations, storage instructions, and a product image carousel.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3, custom `style.css` + per-page stylesheets |
| Layout framework | Bootstrap 5 (`bootstrap.min.css` + `bootstrap.bundle.min.js`) |
| Icons | Bootstrap Icons, Boxicons, RemixIcon |
| Sliders | Slick Slider (jQuery-based) |
| Lightbox | GLightbox |
| Animations | Animate.css |
| Isotope | Isotope Layout (grid filtering) |
| Counters | PureCounter.js |
| Forms | PHP Email Form validation (`validate.js`) |
| Fonts | Google Fonts — Open Sans, Raleway, Poppins |
| Contact backend | PHP (`forms/` directory) |

---

## Project Structure

```
ziniq/
├── index.html
├── produkty.html
├── produkt.html
├── potrzeby-organizmu.html
├── w-co-wierzymy.html
├── gdzie-kupic.html
├── kontakt.html
├── forms/                     # PHP contact form handler
└── assets/
    ├── css/
    │   ├── style.css          # Main stylesheet
    │   └── style-produkt.css  # Product page stylesheet
    ├── js/
    │   └── main.js            # Main JS file
    ├── img/                   # Images, SVG icons, product photos
    │   └── products/          # Product card images
    └── other/                 # Third-party libraries (local copies)
        ├── bootstrap/
        ├── bootstrap-icons/
        ├── boxicons/
        ├── glightbox/
        ├── slick/
        ├── swiper/
        ├── remixicon/
        ├── animate.css/
        ├── isotope-layout/
        ├── purecounter/
        ├── jquery/
        └── php-email-form/
```

---

## Setup & Deployment

The site is fully static (HTML + CSS + JS) with the exception of the contact form, which requires PHP.

### Static hosting (no contact form)

Copy all files to any web server or static hosting service (e.g. Apache, Nginx, GitHub Pages, Netlify). No build step required.

### With contact form

Requires a PHP-enabled server (Apache/Nginx + PHP 7.4+). The `forms/` directory handles form submissions — configure the recipient email address inside the PHP handler before deploying.

### Local preview

Open `index.html` directly in a browser. All assets are referenced with relative paths, so no local server is required for basic browsing. The contact form will not work without a PHP server.

---

## Notes

- All third-party libraries are bundled locally in `assets/other/` — no CDN dependency at runtime.
- The navigation menu is in Polish. The site targets the Polish market.
- Copyright: © 2021 ZiNIQ Sp. z o.o. All rights reserved.

---

## Author

**Przemysław Świerczyński**  
[przemyslaw.swierczynski@o2.pl](mailto:przemyslaw.swierczynski@o2.pl)

---

## License

This project is not under an open-source license. All rights reserved by ZiNIQ Sp. z o.o.
