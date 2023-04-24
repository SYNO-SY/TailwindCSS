# Tailwindcss boilerplate
   - Installing Tailwind CSS as a PostCSS plugin is the most seamless way to integrate it with build tools like webpack, Rollup, Vite, and Parcel.

# Required 
  - [NodeJS](https://nodejs.org/en/download)

# STEP - 01

## Install Tailwind CSS

- Install tailwindcss and its peer dependencies via npm, and create your `tailwind.config.js` file.

- `npx init -y `
- `npm install -D tailwindcss postcss autoprefixer`
- `npx tailwindcss init`

# STEP - 02

1.  Add Tailwind to your PostCSS configuration <br>
1.  Add `tailwindcss` and `autoprefixer` to your `postcss.config.js` file, or wherever PostCSS is configured in your project.

```js
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
};
```

# STEP - 03

## Configure your template paths

- Add the paths to all of your template files in your `tailwind.config.js` file.

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["*"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

# STEP - 04

## Add the Tailwind directives to your CSS

- Add the `@tailwind` directives for each of Tailwind’s layers to your main CSS file.

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

# STEP - 05

## Start your build process

- Run your build process with `npm run dev`

