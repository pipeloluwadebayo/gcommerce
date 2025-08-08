# Dog Meal Landing Page

## Overview

This project is a responsive landing page for a dog food brand, designed to highlight the unique selling points of the product and encourage users to take action. The page is easy to navigate, and structured to communicate the product's benefits clearly.

## Folder Structure

```
gcommerce/
│
├── index.html
├── styles.css
└── assets/
    ├── real-food-icon.png
    ├── premium-ingredient-icon.png
    ├── made-fresh-icon.png
    ├── vet-developed-icon.png
    ├── bowl-split.png
    ├── shield-icon.png
    ├── paypal.png
    ├── visa.png
    ├── mastercard.png
    ├── gpay.png
    └── applepay.png
```

- **index.html**: The main HTML file containing the structure and content of the landing page.
- **style.css**: The CSS file for styling the page and making it responsive.
- **assets/**: Folder containing all image assets used in the landing page.

## Code Explanation

## HTML Code Overview

The `index.html` file structures the Dog Meal landing page and uses a variety of HTML elements to structure and present the content:

- `<!DOCTYPE html>`: Declares the document type and version of HTML.
- `<html lang="en">`: Root element of the page, with language set to English.
- `<head>`: Contains meta information, page title, and links to external resources (like CSS).
  - `<meta charset="UTF-8">`, `<meta name="viewport">`, `<meta http-equiv="X-UA-Compatible">`: Ensure proper character encoding, responsive design, and browser compatibility.
  - `<title>`: Sets the page title shown in the browser tab.
  - `<link rel="stylesheet" href="./style.css">`: Links the external CSS file for styling.

- `<body>`: Contains all visible content on the page.

  - `<div class="title">`  
    - `<h1>`: Main headline for the landing page.

  - `<div class="property">`  
    - Organizes the main feature section into columns.
    - `<div class="child row">`: Left and right columns for features.
      - `<div class="feature">`: Each feature block.
        - `<svg>`: Inline SVG icons for visual representation.
        - `<div class="feature-text">`
          - `<h2>`: Feature title.
          - `<h3>`: Feature description.
    - `<div class="child center-image">`: Center column with a product image.
      - `<img>`: Displays the central product image.

  - `<div class="cta-container">`  
    - Call-to-action section.
    - `<button class="cta-button">`: Main action button.
    - `<div class="payment-logos">`: Payment and guarantee info.
      - `<svg>`: Guarantee icon.
      - `<h4>`: Guarantee text.
      - `<img>`: Payment method logos (PayPal, Visa, MasterCard, Apple Pay, Google Pay).

  - `<div class="section-2">`  
    - Nutrition/info section.
    - `<div class="box text">`: Text content.
      - `<p>`: Section headline.
      - `<h5>`: Supporting text.
      - `<h3>`: Subheading for key points.
      - `<ul>`: List of key statistics.
        - `<li>`: Each statistic.
          - `<h4 class="percentage">`: Percentage/stat value.
          - `<h4>`: Description.
      - `<button class="cta-button">`: Secondary call-to-action.
    - `<div class="box">`: Image box.
      - `<img>`: Image of a dog near food.

  - `<div class="section-3">`  
    - Additional information section.
    - `<div class="top">`: Top row.
      - `<img>`: Animated image of dogs eating.
      - `<div class="text">`
        - `<h3>`: Section headline.
        - `<h5>`: Supporting text.
    - `<div class="bottom">`: Bottom row.
      - `<div class="text">`
        - `<h3>`: Section headline.
        - `<h5>`: Supporting text.
      - `<img>`: Related image (coffee bean).

---

**Summary:**  
The HTML is organized with semantic containers and classes for easy styling and layout. It uses inline SVGs for icons, clear headings, and visually separated sections to guide the user through the page.


## CSS Code Overview

The `styles.css` file provides the layout, typography, and visual styling for the Dog Meal landing page. Here’s a breakdown of the main sections and their purposes

- All icons are inline SVG for easy customization.
- Payment logos and guarantee are shown below the main call-to-action.
- Key stats in the nutrition section are visually emphasized.

### General Styles
- **html, body**: Sets a border and padding, applies the "Inter" font, and uses `box-sizing: border-box` for consistent sizing.

### Layout and Structure
- **.title**: Centers the main title using flexbox and adds padding.
- **.property, .child, .child .row**: Uses flexbox to arrange feature sections and their children for responsive layouts.

### Features Section
- **.feature**: Arranges each feature (icon and text) in a row with spacing and a max width.
- **.feature-text h2, .feature-text h3**: Adds spacing and font size for feature headings.

### Center Image
- **.center-image**: Ensures the central image is displayed as a block element.

### Call to Action (CTA)
- **.cta-container**: Centers the CTA section and stacks its content vertically.
- **.cta-button**: Styles the main action button with color, padding, and rounded corners.

### Payment Logos
- **.payment-logos**: Arranges payment icons in a row with spacing.
- **.payment-logos img**: Sets a consistent size for payment icons.

### Section 2 (Nutrition/Info Section)
- **.section-2**: Creates a two-column layout with a light background.
- **.section-2 .box**: Each column is 50% width.
- **.section-2 .text**: Styles text content with padding and vertical alignment.
- **.section-2 .text p, h5, h3**: Sets font sizes and spacing for headings and paragraphs.
- **.section-2 .text ul, li**: Removes default list styles and aligns list items with flexbox.
- **.section-2 .text ul li h4.percentage**: Highlights key stats in orange and larger font.
- **.section-2 .box img**: Ensures images fill their containers.

### Section 3 (Additional Info)
- **.section-3**: Centers content and limits width for readability.
- **.section-3 .top, .section-3 .bottom**: Arranges content in rows with spacing.
- **.section-3 img**: Limits image width for balance.
- **.section-3 .text, h3, h5**: Adds padding and styles headings for emphasis.

---

**Summary:**  
The CSS uses flexbox for responsive layouts, consistent typography, and visually distinct sections. It ensures the landing page is modern, clean, and easy to navigate.

## How to Run

1. **Clone or Download** this repository.
2. Open `index.html` in your browser.

No build steps or dependencies are required.

## Customization

- **Images:** Replace images in the `/assets` folder as needed.
- **Colors & Fonts:** Adjust in `style.css` to match your brand.
- **SVG Icons:** You can swap out SVG code in `index.html` for your own icons.