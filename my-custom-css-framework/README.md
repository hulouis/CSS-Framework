# CSS-Framework by Chidimma ogborogu

## Overview

This is a custom CSS framework built using **SCSS (Sass)**, with a focus on modular design, reusable components, and utility classes. The framework aims to provide a flexible foundation for building responsive and visually consistent web interfaces.

---

## Table of Contents

- [Getting Started](#getting-started)
- [File Structure](#file-structure)
- [SCSS Architecture](#scss-architecture)
- [Components](#components)
  - [Buttons](#buttons)
  - [Alerts](#alerts)
  - [Cards](#cards)
  - [Forms](#forms)
  - [Modals](#modals)
  - [Navigation](#navigation)
  - [Tables](#tables)
- [Utilities](#utilities)
  - [Backgrounds](#backgrounds)
  - [Colors](#colors)
  - [Layouts](#layouts)
  - [Spacing](#spacing)
  - [Typography](#typography)
- [Customization](#customization)
- [Build Instructions](#build-instructions)
- [Browser Support](#browser-support)

---

## Getting Started

### Prerequisites

To work with this CSS framework, you will need:

- Basic knowledge of HTML and CSS.
- [Sass](https://sass-lang.com/) installed for compiling SCSS files.

### Usage

1. Clone or download the framework to your local machine.
2. Open the `index.html` file to see a sample implementation of the framework.
3. Link the compiled `styles.css` file from the `/dist` directory to your project:
   ```html
   <link rel="stylesheet" href="dist/styles.css" />
   ```

---

## File Structure

```
css-framework/
├── dist/
│   └── styles.css           # Compiled CSS
├── scss/
│   ├── _variables.scss      # Global variables (colors, fonts, etc.)
│   ├── main.scss            # Main SCSS file to import everything
│   ├── base/                # Base styles (resets, typography)
│   ├── components/          # Reusable components (buttons, forms, etc.)
│   └── utilities/           # Utility classes (spacing, layouts, etc.)
└── index.html               # Demo page showcasing the framework
```

---

## SCSS Architecture

The SCSS architecture follows the **7-1 Pattern** to maintain separation of concerns and modularity.

### Global Styles

- **`_variables.scss`**: Contains global variables for colors, fonts, and breakpoints.

### Base Styles

- **`base/_reset.scss`**: Provides a CSS reset to ensure cross-browser consistency.
- **`base/_typography.scss`**: Defines global typography styles.

### Components

Reusable UI components are grouped under the `components` folder for easy import.

- **`_buttons.scss`**: Styles for different button types.
- **`_alerts.scss`**: Alert components for showing notifications.
- **`_cards.scss`**: Card layouts for displaying grouped content.
- **`_forms.scss`**: Styles for form inputs, labels, and buttons.
- **`_modals.scss`**: Modal window styles for popups.
- **`_nav.scss`**: Navigation bar styles for building menus.
- **`_tables.scss`**: Table component styles for displaying tabular data.

### Utilities

Utility classes are small, reusable snippets that make it easy to apply styles without writing custom CSS.

- **`_backgrounds.scss`**: Background color utilities.
- **`_colors.scss`**: Text color utilities.
- **`_layouts.scss`**: Flexbox-based layout utilities.
- **`_spacing.scss`**: Margin and padding utilities.
- **`_typography.scss`**: Utilities for text alignment, font size, and weight.

---

## Components

### Buttons

Buttons come in multiple styles, including primary, secondary, and outline. Example usage:

```html
<button class="btn btn-primary">Primary Button</button>
<button class="btn btn-outline">Outline Button</button>
```

### Alerts

Use alert components to display messages to the user.

```html
<div class="alert alert-success">Success Message</div>
<div class="alert alert-danger">Error Message</div>
```

### Cards

Cards are versatile containers for grouping content.

```html
<div class="card">
  <h3>Card Title</h3>
  <p>Card content goes here.</p>
</div>
```

### Forms

Form components include input fields, buttons, and labels.

```html
<form>
  <label for="name">Name</label>
  <input type="text" id="name" class="form-control" />
  <button class="btn btn-primary">Submit</button>
</form>
```

### Modals

Modals are popups used for dialogs or additional content.

```html
<div class="modal">
  <div class="modal-content">
    <h2>Modal Title</h2>
    <p>Modal body content goes here.</p>
  </div>
</div>
```

### Navigation

The framework provides a basic navigation bar layout.

```html
<nav class="navbar">
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
  </ul>
</nav>
```

### Tables

Style tables for a clean, modern appearance.

```html
<table class="table">
  <thead>
    <tr>
      <th>Name</th>
      <th>Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>John Doe</td>
      <td>28</td>
    </tr>
  </tbody>
</table>
```

---

## Utilities

### Backgrounds

Easily set background colors using utility classes.

```html
<div class="bg-primary">Primary Background</div>
```

### Colors

Change text colors with predefined color classes.

```html
<p class="text-success">Success Text</p>
```

### Layouts

Use Flexbox utilities for creating responsive layouts.

```html
<div class="flex-container">
  <div class="flex-item">Item 1</div>
  <div class="flex-item">Item 2</div>
</div>
```

### Spacing

Control margin and padding with spacing utilities.

```html
<div class="mt-4 mb-2">Content with margin</div>
```

### Typography

Easily adjust text alignment, size, and weight.

```html
<p class="text-center">Centered Text</p>
<p class="font-bold">Bold Text</p>
```

---

## Customization

To customize the framework:

1. Modify the **`_variables.scss`** file to change global settings such as colors, fonts, and breakpoints.
2. Add your own components or utilities by creating new SCSS files in the relevant directories.
3. Recompile the SCSS files into CSS using a Sass compiler.

---

## Build Instructions

1. Install Sass globally on your machine:
   ```bash
   npm install -g sass
   ```
2. Navigate to the root directory of the project:
   ```bash
   cd css-framework/scss
   ```
3. Compile the SCSS to CSS:
   ```bash
   sass main.scss ../dist/styles.css
   ```

---

## Browser Support

This framework is built with modern CSS features and supports the latest versions of all major browsers, including:

- Google Chrome
- Mozilla Firefox
- Safari
- Microsoft Edge

---

## License

This project is open source and available under the [MIT License](LICENSE).
