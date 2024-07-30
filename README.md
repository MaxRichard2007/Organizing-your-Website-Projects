# Organizing Your _SASS_ Projects

For organizing projects using Sass (Syntactically Awesome Stylesheets), a common method for structuring project folders is to use the "7-1 Pattern" principles. This structure helps to divide the Sass files into seven sections and one main file that imports all these sections. This method makes style codes manageable and maintainable.

## Project Structure

```scss
scss/
├── abstracts/
│   ├── _variables.scss
│   ├── _mixins.scss
│   └── _functions.scss
├── base/
│   ├── _reset.scss
│   ├── _typography.scss
│   └── _base.scss
├── components/
│   ├── _buttons.scss
│   ├── _cards.scss
│   └── _forms.scss
├── layout/
│   ├── _header.scss
│   ├── _footer.scss
│   ├── _grid.scss
│   └── _sidebar.scss
├── pages/
│   ├── _home.scss
│   ├── _about.scss
│   └── _contact.scss
├── themes/
│   ├── _theme-dark.scss
│   └── _theme-light.scss
├── vendors/
│   ├── _normalize.scss
│   └── _bootstrap.scss
└── main.scss
```

### _abstracts/_ : 📁

- **This folder contains all the Sass tools and helpers that are used across the project but don't output any CSS directly. These include variables, mixins, and functions.**<br>
  - `_variables.scss`: Stores project-wide variables like colors, fonts, and spacing.
  - `_mixins.scss`: Contains reusable code blocks for styles, like mixins for responsive design or specific styling patterns.
  - `_functions.scss`: Contains custom Sass functions that help with calculations or manipulating values.

### _base/_ : 🧱

- **This folder contains the foundational styles that set the base for the entire project, including CSS resets, base styles, and typography.**<br>
  - `_reset.scss`: Contains styles to reset browser default styles to ensure consistency across different browsers.
  - `_typography.scss`: Defines the base typography styles, such as font families, sizes, and line heights.
  - `_base.scss`: Contains base styles for HTML elements (body, headings, paragraphs, etc.) and general styles that are applied globally.

### _components/_ : 🧩

- **This folder contains styles for small, reusable parts of the UI, known as components, such as buttons, cards, and forms.**<br>
  - `_buttons.scss`: Styles specific to button components.
  - `_cards.scss`: Styles for card components.
  - `_forms.scss`: Styles for form elements and layouts.

### _layout/_ : 📐

- **This folder includes styles for the overall layout and structure of the site, such as grids, header, footer, and sidebar.**<br>
  - `_header.scss`: Styles for the header section of the website.
  - `_footer.scss`: Styles for the footer section.
  - `_grid.scss`: Styles for the grid system used throughout the site.
  - `_sidebar.scss`: Styles for the sidebar or aside components.

### _pages/_ : 📄

- **This folder contains styles specific to individual pages or unique sections of the site.**<br>
  - `_home.scss`: Styles for the homepage.
  - `_about.scss`: Styles for the about page.
  - `_contact.scss`: Styles for the contact page.

### _themes/_ : 🎨

- **This folder includes styles that define different themes, such as dark mode or light mode.**<br>
  - `_theme-dark.scss`: Styles for a dark theme.
  - `_theme-light.scss`: Styles for a light theme.

### _vendors/_ : 🛠️

- **This folder contains third-party styles or libraries, which are either included as is or customized.**<br>
  - `_normalize.scss`: A file for Normalize.css to ensure consistent rendering across browsers.
  - `_bootstrap.scss`: Custom or imported styles from the Bootstrap framework.

### _main.scss_ : 📜

- **The main Sass file that imports all other files. This file is typically used to compile all the styles into a single CSS file. It acts as the central point from which all styles are imported and organized.**

This structured approach helps maintain a clean, organized, and scalable codebase, making it easier to manage and extend as the project grows.
