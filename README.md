# PostCSS

<img align="right" width="95" height="95"
     alt="Philosopher’s stone, logo of PostCSS"
     src="https://postcss.org/logo.svg">

PostCSS is a tool for transforming styles with JS plugins.
These plugins can lint your CSS, support variables and mixins,
transpile future CSS syntax, inline images, and more.

PostCSS is used by industry leaders including Wikipedia, Twitter, Alibaba,
and JetBrains. The [Autoprefixer] and [Stylelint] PostCSS plugins are some of the most popular CSS tools.
# Installation:

``Step 1: ``
Install Tailwind CSS </br>
Install tailwindcss and its peer dependencies via npm, and create your tailwind.config.js file

``` 
npm install -D tailwindcss@3 postcss autoprefixer
npx tailwindcss init
```
``Step 2: ``
Add Tailwind to your PostCSS configuration </br>
Add tailwindcss and autoprefixer to your postcss.config.js file, or wherever PostCSS is configured in your project.

``` postcss.config.js
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  }
}
```
``Step 3: ``
Configure your template paths </br>
Add the paths to all of your template files in your tailwind.config.js file.
```tailwind.config.js
  /** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
``Step 4: ``
Add the Tailwind directives to your CSS </br>
Add the @tailwind directives for each of Tailwind’s layers to your main CSS file.

```main.css
@tailwind base;
@tailwind components;
@tailwind utilities 
```

``Step 5: ``
Start your build process
Run your build process with npm run dev or whatever command is configured in your package.json file
```
npm run dev
```
