# Elevenpacked

A simple Eleventy Starter Kit, my base for all new 11ty projects.

Based of Eleventastic (no external build, maintains manifest.json)

## Features

* CSS Pipeline (SCSS, CleanCSS)
* JS Bundling (Webpack)
* Critical CSS
* HTML Minification
* No external builds, everything runs through 11ty

## Getting Started

To install the necessary packages, run this command in the root folder of the site:

```sh
npm install
```

### Commands

* Run `npm start` for a development server and live reloading
* Run `npm run build` to generate a production build


## CSS

Styling works with SASS/SCSS. The main index file is in src/assets/styles/main.scss. Import any SCSS code you want in there; it will be processed and optimized. The output is in public/assets/styles/main.css.

## JS

Javascript can be written in ES6 syntax. The main index file is in src/assets/scripts/main.js. It will be transpiled to ES5 with babel, bundled together with webpack, and minified in production. The output is in public/assets/scripts/main.js

## Critical CSS

Currently, critical CSS will only be inlined in the head of the homepage. This is done by using the [critical](https://github.com/addyosmani/critical) package in an automatic transform.
