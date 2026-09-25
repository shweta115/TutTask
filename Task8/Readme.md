# 🧺 Laundry Mart – Responsive Laundry Services Landing Page

A responsive **Laundry Services landing page** built using **HTML5 and CSS3** with a **Flexbox-based layout**.

The page presents a laundry service with a navigation bar, logo, username button, service introduction, call-to-action button, laundry image, responsive mobile navigation, and an animated laundry image.

---

## 📌 Project Overview

**Laundry Mart** is a frontend practice project designed to create a clean and responsive laundry service interface.

The page includes:

- Laundry service branding and logo
- Navigation links
- Username/profile button
- Hero section with service information
- "Book a service today!" call-to-action button
- Laundry service image
- Responsive layout for desktop, tablet, and mobile
- Hamburger menu for mobile navigation
- Animated image movement using CSS keyframes

---

## ✨ Features

- 📱 Responsive design
- 🧺 Laundry service landing page
- 🖼️ Laundry-related images
- 🧭 Navigation menu
- 👤 Username button
- 🍔 CSS hamburger menu on mobile
- 📂 Slide-in mobile navigation panel
- 🔘 Call-to-action button
- ✨ Button hover animation
- 🔄 CSS image orbit/movement animation
- 📐 Flexbox layout
- 🎨 Custom colors and styling
- 🔤 Poppins font family
- ⚡ Pure HTML and CSS implementation
- 🚫 No JavaScript or backend required

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Page structure and content |
| CSS3 | Styling, layout, animation, and responsiveness |
| Flexbox | Navigation and main content alignment |
| CSS Media Queries | Desktop, tablet, and mobile layouts |
| CSS Keyframes | Animated movement of the laundry image |
| CSS `:has()` | Opens the mobile navigation when the hamburger checkbox is checked |

---

## 📂 Project Structure

```text
laundry-mart/
│
├── index.html
├── style.css
├── README.md
│
└── img/
    ├── laundry.png
    └── laundry.jpg
```

### File Description

**`index.html`**

Contains the main HTML structure, including:

- Header and navigation
- Laundry logo
- Navigation links
- Username button
- Hamburger menu checkbox and label
- Hero content
- Laundry service description
- Book-service button
- Laundry image

**`style.css`**

Contains:

- Global styling
- Navigation layout
- Flexbox properties
- Typography
- Button styling and hover effect
- Responsive media queries
- Mobile hamburger menu
- Slide-in mobile navigation
- Laundry image animation
- CSS keyframes

**`img/laundry.png`**

Used as the website logo and favicon.

**`img/laundry.jpg`**

Used as the main laundry service image in the hero section.

---

## 🧱 HTML Structure

The main page is organized into the following sections:

```text
<body>
│
├── <header>
│   └── <nav>
│       ├── Logo
│       ├── Navigation Menu
│       ├── Username Button
│       └── Hamburger Menu
│
└── <main>
    └── .container
        ├── .left
        │   ├── Heading
        │   ├── Subheading
        │   ├── Description
        │   └── Book Service Button
        │
        └── .right
            └── Laundry Image
```

---

## 🎨 Design and Styling

The design uses a clean laundry-service theme.

### Main Colors

- Heading: `#585252`
- Primary blue: `#06A8FF`
- Secondary blue: `#3BB8F0`
- Username background: `#EAF6FD`
- Username text: `#3299CF`
- Mobile menu background: `#2b2a2a`
- General text: `grey`
- Page background: `#fff`

### Typography

The stylesheet uses:

```css
font-family: 'Poppins', sans-serif;
```

---

## 📐 Flexbox Layout

Flexbox is used throughout the page for positioning and alignment.

For example, the main container uses:

```css
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
```

The left and right sections each use flexible layouts to arrange the content and image.

The navigation also uses Flexbox:

```css
nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
}
```

---

## 📱 Responsive Design

The stylesheet contains separate responsive rules for tablet and mobile screens.

### Desktop

The main content is arranged horizontally:

- Left side: laundry service content
- Right side: laundry image
- Horizontal navigation menu
- Username button

### Tablet

For screens between `768px` and `1033px`:

- Main container height is reduced
- Left section uses `60vw`
- Right section uses `40vw`
- Font sizes and line heights are adjusted
- Button and spacing are reduced

### Mobile

For screens between `360px` and `767px`:

- Main content changes to a column layout
- Navigation links are hidden initially
- Hamburger icon is displayed
- Laundry image width becomes `70vw`
- Heading and paragraph sizes are adjusted
- Navigation becomes a slide-in side panel

---

## 🍔 Hamburger Menu

The mobile navigation is implemented without JavaScript.

The HTML uses a hidden checkbox:

```html
<input type="checkbox" id="menu-toggle">
<label for="menu-toggle" class="hamburger">
    <span></span>
    <span></span>
    <span></span>
</label>
```

When the checkbox is checked, CSS opens the navigation panel using:

```css
nav:has(#menu-toggle:checked) .bar {
    right: 0;
}
```

The menu slides in from the right side of the screen.

The mobile menu has:

- `65vw` width
- `100%` height
- Dark background
- Vertical navigation links
- CSS transition effect

---

## 🔘 Book a Service Button

The main call-to-action button is:

```html
<button class="book">Book a service today!</button>
```

It uses a blue gradient:

```css
.book {
    background: linear-gradient(to right, #06A8FF, #3BB8F0);
    color: #FFFFFF;
    border: 0;
    border-radius: 2vh;
    cursor: pointer;
}
```

### Hover Effect

When the user hovers over the button, it rotates and scales:

```css
.book:hover {
    transform: rotate(-10deg) scalex(1.5);
    transition: transform 0.6s ease-in;
}
```

The current implementation provides a visual hover interaction; the button does not submit a form or navigate to another page.

---

## 🔄 Laundry Image Animation

The laundry image uses CSS animation:

```css
.right > img {
    animation-name: orbit;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
}
```

The `@keyframes orbit` rule moves the image through several positions:

```text
Top
  ↓
Upper-right
  ↓
Right
  ↓
Lower-right
  ↓
Bottom
  ↓
Lower-left
  ↓
Left
  ↓
Upper-left
  ↓
Top
```

This creates a continuous orbit-like movement using CSS `transform: translate()` values.

The animation also includes a small scale transformation at one keyframe.

---

## 🚀 How to Run the Project

### 1. Download or clone the project

```bash
git clone <repository-url>
```

### 2. Open the project folder

```bash
cd laundry-mart
```

### 3. Check the image folder

Make sure the following files are available:

```text
img/
├── laundry.png
└── laundry.jpg
```

### 4. Open the webpage

Open:

```text
index.html
```

in a modern web browser.

You can also open the project directly using **Visual Studio Code** and its Live Server extension.

---

## 🌐 Browser Support

The project is intended for modern browsers such as:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

The mobile menu uses the CSS `:has()` selector, so a modern browser is recommended.

---

## 📋 Requirements

No backend, database, or JavaScript framework is required.

You only need:

- A modern web browser
- A code editor such as Visual Studio Code
- The project image files

---

## 👩‍💻 Learning Objectives

This project demonstrates practical knowledge of:

- HTML5 semantic structure
- CSS3 styling
- Flexbox
- Responsive web design
- Media queries
- CSS hover effects
- CSS transitions
- CSS animations
- `@keyframes`
- CSS transforms
- Checkbox-based UI interaction
- CSS `:has()` selector
- Image handling
- Navigation design
- Mobile-first interaction concepts
- Project organization

---

## 📄 License

This project is created for **learning and frontend development practice**.

You are free to modify and extend it for personal or educational purposes.

---

## 🧺 Laundry Mart

**Simple • Clean • Responsive • User-Friendly**

A responsive laundry service landing page built with **HTML5 + CSS3 + Flexbox**, featuring a CSS-powered mobile menu and animated laundry image.
