# One Layout, Three Screens: LearnLoop Course Catalog Grid

A fully responsive, production-ready course-catalog grid built for the Week 1 Frontend assignment. This project demonstrates true mobile-first responsive adaptation rather than simple scaling, using modern CSS features **without any JavaScript**.

---

## 🚀 Live Preview / Repository
- **GitHub Repository:** [Insert your GitHub repo link here]

---

## 🛠️ Technical Highlights & Stack
- **Semantic HTML5:** Built using clean semantic tags (`<header>`, `<main>`, `<section>`, `<article>`, `<picture>`).
- **CSS Grid:** Implemented with responsive column layouts (`1fr`, `repeat(2, 1fr)`, and `repeat(3, 1fr)`).
- **Pure CSS Interactive Filtering:** Uses hidden radio inputs and sibling selectors to achieve real-time filtering without JavaScript.
- **Responsive Images:** Utilizes `<picture>` and `<source>` elements with strict `aspect-ratio: 16/9` to prevent cumulative layout shifts across breakpoints.
- **Fluid Typography:** Scales headlines and pricing seamlessly across viewports using CSS `clamp()`.

---

## 📱 Responsive Comparison Table

| Breakpoint Range | Grid Columns | Filter Bar Layout | Image Treatment (`<picture>` / Aspect Ratio) | Typography Scale (`clamp()`) |
| :--- | :--- | :--- | :--- | :--- |
| **Mobile** (<600px) | **1 Column** (`1fr`) | Collapsed into a vertical **stacked list** of full-width buttons for thumb-friendly interaction. | Uses mobile-optimized source asset with a fixed `aspect-ratio: 16/9` using `object-fit: cover`. | Scaled down smoothly using lower `clamp()` limits to prevent text overflowing. |
| **Tablet** (600px–1023px) | **2 Columns** (`repeat(2, 1fr)`) | Transitions into a **horizontal row** layout for efficient space utilization. | Switches via media query to medium-res asset while maintaining the consistent `16/9` ratio. | Mid-range fluid sizing scaling dynamically with the viewport width. |
| **Desktop** (≥1024px) | **3 Columns** (`repeat(3, 1fr)`) | Full horizontal layout featuring an added **visible sort dropdown placeholder**. | High-resolution image sources loaded with strict `16/9` constraint to keep visual balance. | Maximum `clamp()` headline and price scaling for a professional hierarchy. |

---

## 📂 Project Structure
```text
├── index.html         # Main markup file containing 9 course cards & filter controls
├── styles.css         # Complete styling, CSS grid, breakpoints, and pure CSS filtering logic
├── README.md          # Project documentation and comparison table
└── screenshots/       # Contains responsive breakpoint captures
    ├── mobile.png
    ├── tablet.png
    └── desktop.png