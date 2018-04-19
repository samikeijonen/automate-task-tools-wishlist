# Automate task tools wishlist

This is my automate task tools wishlist. You could use [Gulp](https://gulpjs.com/), [Grunt](https://gruntjs.com/), [Webpack](https://webpack.js.org/), or something else.

## Watching the files and having BrowserSync

Browser should re-load automatically when CSS, SVG, image, PHP, or other project files are changed. [BrowserSync](https://browsersync.io/) is also usefull for testing the site in different browsers and devices.

## SASS support

Task tools should be able to compile SASS files. Output file should be run through autoprefixer and minified. There should also be sourcemaps in the dev environment.

At the moment every main `*.scss` I have in `styles` folder gets outputted automatically. For example I want different file for just in the editor (Gutenberg):

```
styles/editor.scss
styles/style.scss
```

These files would be outputted automatically as:

```
dist/style.css
dist/style.min.css
dist/editor.min.css
dist/editor.min.css
```

`*.min.css` file is the minified file which is loaded in production. `*.css` is the non-minified file with sourcemaps, and is loaded in development environment.

## Javascript support

Pretty much the same as SASS but all Javascript can be probably concatenated in one file. 

- Also JS needs sourcemaps for easier debugging.
- JS should be run through Babel if and when ES6 is used.
- How would we load 3th party scripts? Own folder for them or?

## Optimize images

Well, optimize images and output in `dist` folder.

## Optimize SVGs

Well, optimize SVGs and output in `dist` folder. Also add class `icon icon-{icon-name}`.

## Linting

- SASS linting using `stylelint`.
- JS linting using `eslint`.
- PHP linting using PHP codesniffer.
- HTML linting using HTMl codesniffer.

## Sass docs

Creating SASS docs automatically.



