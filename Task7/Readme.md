# 🧺 Laundry Mart – Responsive Laundry Services App

A simple and responsive **Laundry Services landing page** built using **HTML5, CSS3, and Flexbox**.

The project is designed to provide a clean and user-friendly interface for a laundry service website. It includes a responsive layout, laundry service imagery, service information, and an interactive call-to-action button/form.

---

## 📌 Project Overview

**Laundry Mart** is a responsive laundry service webpage created as a frontend practice project.

The website focuses on:

* Clean and modern UI
* Responsive design
* Laundry service presentation
* User interaction
* Flexbox-based layout
* Mobile-friendly design

---

## ✨ Features

* 📱 Fully responsive design
* 🧺 Laundry service landing page
* 🖼️ Laundry-related image
* 🔘 Interactive CTA button
* 📝 Laundry service form
* 📐 Flexbox layout
* 🎨 Custom colors and styling
* 🔤 Custom typography
* 📱 Mobile, tablet, and desktop support
* ⚡ Lightweight HTML and CSS implementation

---

## 🛠️ Technologies Used

| Technology    | Purpose                       |
| ------------- | ----------------------------- |
| HTML5         | Page structure and content    |
| CSS3          | Styling and responsive design |
| Flexbox       | Layout and alignment          |
| Media Queries | Responsive behavior           |

---

## 📂 Project Structure

```text
laundry-mart/
│
├── index.html
│
├── style.css
│
├── README.md
│
└── img/
    └── laundry.png
```

### File Description

**`index.html`**
Contains the main structure and content of the Laundry Mart webpage.

**`style.css`**
Contains all styling, Flexbox layout, responsive rules, colors, typography, buttons, and form styling.

**`img/laundry.png`**
Contains the laundry service image used on the webpage.

**`README.md`**
Contains project documentation and setup instructions.

---

## 🎨 Design

The design uses a clean laundry-service theme with:

* Light background
* Laundry-related imagery
* Highlighted CTA button
* Rounded UI elements
* Clear typography
* Responsive spacing
* Flexbox-based alignment

The layout adapts according to the available screen size.

---

## 📱 Responsive Design

The webpage is designed to work across different devices:

### Desktop

* Two-column/flexible layout
* Larger image and content area
* Horizontal form elements where appropriate

### Tablet

* Adjusted spacing and sizing
* Flexible content arrangement

### Mobile

* Content stacks vertically
* Form fields adapt to screen width
* Buttons become easier to tap
* Images scale according to viewport width

CSS media queries are used to handle different screen sizes.

---

## 🧩 Flexbox Implementation

Flexbox is used for arranging and aligning the main page elements.

Example:

```css
.container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 30px;
}
```

For smaller screens, the layout can switch to a vertical arrangement:

```css
@media (max-width: 768px) {
    .container {
        flex-direction: column;
    }
}
```

---

## 🔘 Button Interaction

The CTA button provides a clear action for the user.

Example styling:

```css
.cta-button {
    background: linear-gradient(90deg, #ff4b4b, #ff6b6b);
    color: #ffffff;
    border: none;
    padding: 12px 24px;
    border-radius: 6px;
    cursor: pointer;
    font-size: 16px;
}
```

A hover effect can be added to improve user interaction:

```css
.cta-button:hover {
    transform: scale(1.03);
}

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

### 3. Open `index.html`

You can simply double-click:

```text
index.html
```

or open it using a browser.

---

## 🌐 Browser Support

The project works with modern browsers including:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Safari

---

## 📋 Requirements

No backend or database is required.

You only need:

* A modern web browser
* A code editor such as VS Code

---

## 👩‍💻 Learning Objectives

This project demonstrates practical knowledge of:

* HTML semantic structure
* CSS styling
* Flexbox
* Responsive web design
* Media queries
* Forms
* Buttons and hover states
* Image handling
* Project organization

---

## 📄 License

This project is created for **learning and frontend development practice**.

You are free to modify and extend it for personal or educational purposes.

---

## 🧺 Laundry Mart

**Simple • Clean • Responsive • User-Friendly**

A responsive laundry service interface built with **HTML5 + CSS3 + Flexbox**.
