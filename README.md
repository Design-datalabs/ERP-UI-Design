# Reusable Navbar for Crest ERP System

This project provides a reusable navbar component for the Crest ERP System. The navbar is designed to be easily integrated into any page of the ERP system, ensuring a consistent navigation experience across the application.

## Features

- **Modern Design**: Clean, professional navbar with responsive layout
- **Dropdown Menus**: Multi-level dropdown menus for organized navigation
- **Active Menu Highlighting**: Automatically highlights the active menu item based on the current page
- **User Profile**: Includes a user profile section with logout functionality
- **Mobile Responsive**: Works well on all screen sizes, from desktop to mobile
- **Easy Integration**: Simple to add to any page with minimal code

## How to Use

### 1. Include Required Files

Make sure the following files are in your project:
- `navbar.html` - Contains the navbar HTML structure
- `loadNavbar.js` - JavaScript that loads the navbar into any page
- `index.css` - CSS styles for the navbar

### 2. Add to Your Page

To add the navbar to any page, follow these steps:

1. Include the required CSS and JavaScript files in your HTML:

```html
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- Bootstrap Icons -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.1/font/bootstrap-icons.css">

<!-- Custom CSS -->
<link rel="stylesheet" href="index.css">
```

2. Add a placeholder div for the navbar:

```html
<!-- Navbar placeholder - will be filled by loadNavbar.js -->
<div id="navbar-placeholder"></div>
```

3. Include the JavaScript file at the end of your body tag:

```html
<!-- Bootstrap JS Bundle with Popper -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

<!-- Load Navbar Script -->
<script src="loadNavbar.js"></script>
```

That's it! The navbar will be automatically loaded into the placeholder div when the page loads.

## Customization

### Changing the Logo

To change the logo, edit the `navbar.html` file and update the image source:

```html
<a class="navbar-brand" href="#">
    <img src="path/to/your/logo.png" alt="Your Logo" height="40">
</a>
```

### Adding or Modifying Menu Items

To add or modify menu items, edit the `navbar.html` file. The navbar uses Bootstrap's dropdown menu structure:

```html
<li class="nav-item dropdown">
    <a class="nav-link" href="#">MENU ITEM</a>
    <ul class="dropdown-menu">
        <li><a class="dropdown-item" href="#">Submenu Item 1</a></li>
        <li><a class="dropdown-item" href="#">Submenu Item 2</a></li>
    </ul>
</li>
```

For nested dropdowns (dropdowns within dropdowns), use the `dropdown-submenu` class:

```html
<li class="dropdown-submenu">
    <a class="dropdown-item" href="#">Nested Menu <i class="bi bi-chevron-right ms-1"></i></a>
    <ul class="dropdown-menu">
        <li><a class="dropdown-item" href="#">Nested Item 1</a></li>
        <li><a class="dropdown-item" href="#">Nested Item 2</a></li>
    </ul>
</li>
```

### Styling

To customize the appearance of the navbar, edit the `index.css` file. The CSS includes styles for:

- Navbar container and layout
- Navigation links and dropdowns
- User profile section
- Responsive design adjustments

## Example

See the `example-page.html` file for a complete example of how to use the navbar in a page.

## Browser Support

The navbar is compatible with all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

## License

This project is part of the Crest ERP System and is intended for use within that system only. 