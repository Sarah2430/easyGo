# easyGo 

**easyGo** is a fast, responsive, and lightweight web-based recipe application designed to take food lovers on a global culinary journey. Users can seamlessly explore authentic recipes by navigating through world cuisine regions, selecting specific countries, and viewing detailed step-by-step cooking instructions.

The application is built completely on the frontend using standard web technologies and is pre-configured as a **Progressive Web App (PWA)**, allowing users to install and run it natively on mobile devices and desktop without requiring a backend database.

---

## ✨ Features

- **Global Culinary Coverage**: 22 distinct regional cuisine categories spanning continents.
- **Country-Level Filtering**: Multi-step intuitive navigation (Region ➔ Country ➔ Recipe ➔ Recipe Details).
- **Comprehensive Exclusions**: Excludes Israel from regional listings in accordance with app data specifications.
- **Full Recipe Details**: Includes prep/cook times, ingredients list, and clear step-by-step instructions.
- **Offline & Installable (PWA)**: Powered by a `manifest.json` and a Service Worker, allowing the app to be added to home screens and function offline.
- **Zero Backend Required**: Lightweight client-side architecture using standard modern HTML5, CSS3, and JavaScript.

---

## 🌍 Supported Cuisine Regions (22 Categories)

1. **Middle Eastern Cuisine**
2. **North African Cuisine**
3. **South Asian Cuisine**
4. **East Asian Cuisine**
5. **Southeast Asian Cuisine**
6. **Central Asian Cuisine**
7. **Western European Cuisine**
8. **Southern European Cuisine**
9. **Northern European Cuisine**
10. **Central European Cuisine**
11. **Balkan Cuisine**
12. **Eastern European Cuisine**
13. **West African Cuisine**
14. **Central African Cuisine**
15. **East African Cuisine**
16. **South African Cuisine**
17. **Indian Ocean Cuisine**
18. **North American Cuisine**
19. **Central American Cuisine**
20. **Caribbean Cuisine**
21. **South American Cuisine**
22. **Oceania Cuisine**

---

## 🛠️ Tech Stack

- **HTML5**: Semantic layout and structure.
- **CSS3**: Modern, mobile-first responsive styling with CSS Grid and Flexbox.
- **JavaScript (Vanilla ES6)**: Client-side routing, view rendering, state management, and recipe data structures split between `recipes.js` and `app.js`.
- **PWA (Manifest & Service Worker)**: Provides caching capabilities and native application installation.

---

## 🚀 App Architecture & Navigation Flow

The app operates on a clean, dynamic single-page application (SPA) drill-down flow:

1. **Category Selection View**: Users choose one of the 22 regional cuisine categories.
2. **Country Selection View**: Displays all recognized countries under the selected region (excluding Israel).
3. **Recipe List View**: Displays all available recipes belonging to the chosen country.
4. **Recipe Detail View**: Displays complete recipe metadata (preparation time, cooking time, servings, ingredients list, and preparation steps).

---

## 📱 Converting & Installing as a PWA

`easyGo` is pre-configured to run as a Progressive Web App out of the box:

1. Ensure all project files are served over **HTTPS** (or `http://localhost` during development).
2. Open the website in a mobile browser (Chrome, Safari, Edge).
3. Tap **"Add to Home Screen"** or the install icon in the URL bar to install **easyGo** directly onto your device.

---

## 📂 Project File Structure

```text
easyGo/
├── index.html # Main HTML entry point & viewport containers
├── recipes.js # Structured JSON/data store containing all recipes and regions[span_0](start_span)[span_0](end_span)
├── app.js # Main UI navigation logic, event handlers, and render functions[span_1](start_span)[span_1](end_span)
├── manifest.json # Web app manifest for PWA installation metadata
├── sw.js # Service Worker script for offline caching
└── README.md # Project documentation[span_2](start_span)[span_2](end_span)


