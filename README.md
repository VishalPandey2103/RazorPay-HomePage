# Razorpay Homepage Clone

A responsive frontend recreation of the **Razorpay homepage**, built to practice modern frontend development, responsive layouts, Tailwind CSS, UI composition, and landing-page design.

The project recreates the visual structure and major sections of a Razorpay-style payment platform landing page using **HTML, Tailwind CSS, Vite, and Feather Icons**.

## Overview

This project focuses on reproducing the frontend experience of a modern fintech landing page.

The page includes:

* Promotional announcement banner
* Responsive navigation bar
* Hero section
* Payment gateway section
* Payment feature cards
* Banking and financial product sections
* Business-focused feature sections
* Interactive hover effects
* Call-to-action sections
* Responsive layouts
* Custom illustrations and SVG assets
* Footer/navigation content

The implementation is primarily contained in `index.html`, with styling supported by Tailwind CSS and `style.css`.

---

# Tech Stack

| Technology    | Purpose                                      |
| ------------- | -------------------------------------------- |
| HTML5         | Page structure and semantic markup           |
| Tailwind CSS  | Utility-first styling and responsive layouts |
| CSS3          | Additional/custom styling                    |
| Vite          | Development server and production build      |
| Feather Icons | UI icons                                     |
| PostCSS       | CSS processing                               |
| JavaScript    | Client-side UI/icon functionality            |

The project's `package.json` uses Vite 4.1.1, Tailwind CSS 3.4.17, PostCSS, Autoprefixer, and Feather Icons.

---

# Features

## 1. Promotional Banner

The top of the page contains a promotional announcement banner styled using Tailwind utility classes and geometric CSS shapes.

It includes a promotional message and a **Know More** call-to-action.

---

## 2. Navigation Bar

The navigation bar contains:

```text
Razorpay Logo
    |
    +── Payments
    +── Banking
    +── Corporate Card
    +── Payroll
    +── Resources
    +── Support
    +── Pricing
    |
    +── Login
    +── Sign Up
```

The navigation uses Tailwind classes for spacing, typography, colors, hover effects, and positioning.

---

## 3. Hero Section

The hero section establishes the primary purpose of the page.

It contains:

* Main headline
* Supporting description
* Sign Up CTA
* Hero illustration
* Decorative curved/shape element

The hero content communicates the idea of helping businesses accept payments, automate payouts, and manage working capital.

---

## 4. Payment Gateway Section

The page contains a dedicated payment-suite section presenting a payment gateway as the main product.

It highlights capabilities such as:

* 100+ payment methods
* High payment success rate
* Checkout experience
* Easy integration
* Instant settlements
* Reporting and insights

The section combines text, CTA buttons, feature lists, and visual assets.

---

## 5. Payment Feature Cards

The payment section contains multiple feature cards representing different payment products.

Examples include:

```text
Payment Links
Payment Pages
Payment Buttons
Subscriptions
Route
```

Each card contains an icon, title, description, and **Know More** action.

The cards also use hover-based visual transitions.

---

## 6. Interactive Hover Effects

The page uses CSS transitions and Tailwind utility classes to create interactive UI effects.

For example, feature cards change their visual appearance when the user hovers over them.

The project also uses custom CSS rules for feature-card icons, SVG effects, shadows, gradients, and background illustrations.

---

# Project Structure

```text
RazorPay-HomePage/
│
├── Images/
│   ├── logo.svg
│   ├── india-flag.svg
│   ├── hero-illustration.jpg
│   ├── hero-shape.svg
│   ├── payment-suite.png
│   ├── payment-link-icon.svg
│   ├── payment-pages-icon.svg
│   ├── payment-button.svg
│   ├── subscriptions-icon.svg
│   ├── route-icon.svg
│   └── ...
│
├── index.html
├── style.css
├── package.json
├── package-lock.json
├── tailwind.config.js
├── postcss.config.js
└── .gitignore
```

The repository currently contains the main HTML page, CSS, Tailwind configuration, PostCSS configuration, package files, and an `Images` directory containing the visual assets used by the page.

---

# How It Works

The application is a static frontend rather than a backend application.

The high-level flow is:

```text
Browser
   |
   v
index.html
   |
   +── HTML structure
   |
   +── Tailwind CSS classes
   |
   +── style.css
   |
   +── Images / SVG assets
   |
   +── Feather Icons
   |
   v
Rendered Razorpay-style Homepage
```

There is no server-side API or database involved in the current implementation.

The project uses Vite as the development/build tool. The `start` script launches Vite, while the `build` script generates a production build.

---

# Styling Approach

The majority of the page styling is implemented using **Tailwind CSS utility classes directly inside the HTML**.

For example:

```html
<section class="relative text-white">
```

and:

```html
<div class="w-11/12 mx-auto max-w-[1080px]">
```

This approach allows layout, spacing, typography, colors, positioning, and responsive behavior to be expressed directly alongside the HTML structure.

Custom CSS is also used where more specific styling or animation is required.

Examples include:

```css
@keyframes moving {
  0% {
    top: 0;
  }

  100% {
    top: -50%;
  }
}
```

The page also contains custom hover rules for feature cards and their icons.

---

# Icons

The project uses **Feather Icons** for several interface elements.

The Feather Icons library is loaded in the HTML:

```html
<script src="https://unpkg.com/feather-icons"></script>
```

Icons are then represented using attributes such as:

```html
<i data-feather="check"></i>
```

and:

```html
<i data-feather="chevron-right"></i>
```

This keeps the interface lightweight while providing consistent vector-based icons.

---

# Responsive Design

The page uses Tailwind's responsive utility classes to adapt the layout across different screen sizes.

Examples include:

```text
lg:
md:
w-full
w-11/12
max-w-[1080px]
grid-cols-3
```

The layout uses constrained container widths and responsive positioning to maintain the desktop landing-page structure while adapting elements for smaller screens.

---

# Installation

## Prerequisites

Make sure the following are installed:

* Node.js
* npm

## Clone the Repository

```bash
git clone https://github.com/VishalPandey2103/RazorPay-HomePage.git
```

Navigate into the project:

```bash
cd RazorPay-HomePage
```

## Install Dependencies

```bash
npm install
```

---

# Run Locally

Start the Vite development server:

```bash
npm start
```

The project defines the following Vite script:

```json
{
  "scripts": {
    "start": "vite",
    "build": "vite build"
  }
}
```

Vite will display the local development URL in the terminal.

---

# Production Build

To generate an optimized production build:

```bash
npm run build
```

This executes:

```bash
vite build
```

and generates the production-ready output.

---

# Design Highlights

The project focuses on reproducing several common patterns used in modern SaaS and fintech landing pages.

### Component-like Sections

Although the project does not use React components, the HTML is organized into logically separated sections:

```text
Announcement Banner
        ↓
Navigation
        ↓
Hero
        ↓
Payment Suite
        ↓
Feature Cards
        ↓
Business/Banking Sections
        ↓
CTA
        ↓
Footer
```

### Visual Hierarchy

The page uses:

* Large hero typography
* Strong contrast between dark and light sections
* Blue as the primary accent color
* Card-based feature presentation
* Large product illustrations
* CTA buttons
* Decorative SVG shapes

These elements create a visual hierarchy similar to modern financial-product landing pages.

---

# Learning Objectives

This project demonstrates practical frontend concepts including:

* HTML page structuring
* Tailwind CSS
* Responsive design
* Flexbox
* CSS Grid
* Utility-first CSS
* SVG integration
* Image optimization/loading
* Hover states
* CSS transitions
* CSS animations
* Landing-page composition
* Vite development workflow
* Asset organization

---

# Future Improvements

Possible improvements include:

* Convert the static HTML into reusable React components.
* Add fully functional navigation links.
* Implement mobile navigation with a hamburger menu.
* Add actual button interactions.
* Improve accessibility with semantic elements and ARIA attributes where appropriate.
* Add more robust responsive behavior for smaller screens.
* Add deployment using GitHub Pages, Vercel, or Netlify.
* Add a live demo link.
* Optimize and lazy-load all non-critical assets.
* Add automated linting and formatting.
* Separate large sections of `index.html` into reusable components if migrating to React.

---

# Disclaimer

This project is a **frontend learning project and visual recreation** inspired by the Razorpay website.

It is not an official Razorpay product or application and does not implement Razorpay's actual payment processing infrastructure.

No real payment processing is performed by this project.

---

# Author

**Vishal Pandey**

GitHub: [VishalPandey2103](https://github.com/VishalPandey2103)

Repository: [RazorPay-HomePage](https://github.com/VishalPandey2103/RazorPay-HomePage)
