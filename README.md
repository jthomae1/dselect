# dselect Fork

Dropdown select box for bootstrap 5 - A customizable dropdown select box built for Bootstrap 5, enhanced with additional flexibility for the `Creatable` feature.
This repository is a fork of the original [dselect](https://github.com/jarstone/dselect) project.

## Overview

This version of dselect brings you the same great features, including placeholder text, multiple selections, search functionality, and more. Plus, enjoy the ability to create new options dynamically!

## Key Features

- **Placeholder Support**: Easily set a placeholder for your select box.
- **Multiple Selection**: Enable multiple selections at once.
- **Search Feature**: Quickly find items in large lists.
- **Creatable Options**: Add new options on-the-fly.
- **Clearable**: Simplify selection clearing.
- **Dynamic Sizing**: Adjust component size with ease.
- **Built-in Validation**: Ensure data integrity.

## Installation

Install dselect with npm

```bash
npm install @jthomae1/dselect
```

Install from cdn
```html
<link rel="stylesheet" href="https://unpkg.com/@jthomae1/dselect/dist/css/dselect.css">
<script src="https://unpkg.com/@jthomae1/dselect/dist/js/dselect.js"></script>
```

## Quick Start
Here's how to quickly set up dselect in your project:

### HTML

```html
<select class="form-select" id="dselect-example">
    <option value="chrome">Chrome</option>
    <option value="firefox">Firefox</option>
    <option value="safari">Safari</option>
    <option value="edge">Edge</option>
    <option value="opera">Opera</option>
    <option value="brave">Brave</option>
</select>
```

### JavaScript

```javascript
dselect(document.querySelector('#dselect-example'))
```

## Configuration Options
Customize dselect with these options:

```javascript
const config = {
    search: false, // Toggle search feature. Default: false
    creatable: false, // Creatable selection. Default: false
    clearable: false, // Clearable selection. Default: false
    maxHeight: '360px', // Max height for showing scrollbar. Default: 360px
    size: '', // Can be "sm" or "lg". Default ''
}
dselect(document.querySelector('#dselect-example'), config)
```

### Inline Configuration

Options can also be set directly in the HTML using `data-dselect-*` attributes:

```html
<select data-dselect-search="true" data-dselect-creatable="true" data-dselect-clearable="true" data-dselect-max-height="300px" data-dselect-size="sm" class="form-select" id="dselect-example">
...
</select>
```

## Changes and Improvements

This fork introduces enhancements to the dropdown functionality, including improved search and creation capabilities. Previously, the dropdown restricted adding new entries if they started with existing item letters, causing limitations for users. The updated logic now allows for any new values to be added unless they exactly match an existing entry and have at least three letters, thereby expanding on the original functionality. These improvements ensure a more flexible and user-friendly experience. The changes can be tested by downloading the repository and opening the [index.html](https://github.com/jthomae1/dselect/blob/main/dist/index.html) in a browser of your choice. 

Additionally, some dependencies in the `package.json` were updated.

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues](https://github.com/jthomae1/dselect/issues) page and submit new ideas.

## License

This project is licensed under the MIT License. See the [LICENSE](https://github.com/jthomae1/dselect/blob/main/LICENSE) file for more details.
