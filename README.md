# Custom CSS Library Documentation

This documentation provides an overview and usage guide for the custom CSS library. The library includes styles for containers, grids, cards, buttons, forms, badges, and tables.

## Table of Contents

1. [Container](#container)
2. [Grid System](#grid-system)
3. [Cards](#cards)
4. [Buttons](#buttons)
5. [Forms](#forms)
6. [Badges](#badges)
7. [Tables](#tables)
8. [Responsive Design](#responsive-design)

## Container

The container class provides a responsive fixed-width container for your content.

Usage:

```html
<div class="container">
  <!-- Your content here -->
</div>
```

## Grid System

The library includes a 12-column grid system for flexible layouts.

Usage:

```html
<div class="row">
  <div class="col-6">Half width column</div>
  <div class="col-6">Half width column</div>
</div>

<div class="row">
  <div class="col-4">One-third width column</div>
  <div class="col-4">One-third width column</div>
  <div class="col-4">One-third width column</div>
</div>
```

Available column classes:
- `col-1` to `col-12`: Specify column width (e.g., `col-6` for 50% width)
- `col`: Equal-width column

## Cards

Cards are flexible content containers.

Usage:

```html
<div class="card">
  <h2 class="card-title">Card Title</h2>
  <p class="card-content">This is the card content.</p>
</div>
```

## Buttons

The library provides styles for buttons.

Usage:

```html
<button class="btn btn-primary">Primary Button</button>
<button class="btn btn-secondary">Secondary Button</button>
```

Available button classes:
- `btn`: Base button class
- `btn-primary`: Primary action button
- `btn-secondary`: Secondary action button

## Forms

Form styles for input fields and labels.

Usage:

```html
<form>
  <div class="form-group">
    <label class="form-label" for="username">Username</label>
    <input class="form-input" type="text" id="username" name="username">
  </div>
  <div class="form-group">
    <label class="form-label" for="password">Password</label>
    <input class="form-input" type="password" id="password" name="password">
  </div>
  <button class="btn btn-primary" type="submit">Submit</button>
</form>
```

## Badges

Badges can be used to add small labels to other elements.

Usage:

```html
<span class="badge badge-primary">New</span>
<span class="badge badge-secondary">Updated</span>
```

Available badge classes:
- `badge`: Base badge class
- `badge-primary`: Primary badge style
- `badge-secondary`: Secondary badge style

## Tables

Styled tables for displaying tabular data.

Usage:

```html
<table class="table">
  <thead>
    <tr>
      <th>Header 1</th>
      <th>Header 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Row 1, Cell 1</td>
      <td>Row 1, Cell 2</td>
    </tr>
    <tr>
      <td>Row 2, Cell 1</td>
      <td>Row 2, Cell 2</td>
    </tr>
  </tbody>
</table>
```

## Responsive Design

The library includes basic responsive design features:

- The grid system collapses to full-width columns on small screens (below 768px).
- The container adapts its width based on the screen size.

To ensure proper responsive behavior, always include the viewport meta tag in your HTML:

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

## Customization

To customize the library, you can modify the CSS variables or override specific styles. It's recommended to create a separate CSS file for your customizations and load it after the main library CSS.

Example customization:

```css
/* custom-styles.css */
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
}

.btn-primary {
  background-color: var(--primary-color);
}

.btn-secondary {
  background-color: var(--secondary-color);
}
```

Then include both CSS files in your HTML:

```html
<link rel="stylesheet" href="path/to/custom-library.css">
<link rel="stylesheet" href="path/to/custom-styles.css">
```

This documentation should help you get started with using and customizing the CSS library. Feel free to expand upon this foundation to meet your specific project needs.
