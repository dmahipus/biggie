# biggie
Biggie is a JavaScript application boilerplate written in ES6 based on [bigwheel](https://github.com/bigwheel-framework), a minimalist framework from [Jam3](http://www.jam3.com/).
Be sure to check out the full [documentation](https://github.com/bigwheel-framework/documentation) for bigwheel before you're getting started.

## Getting Started

`git clone https://github.com/baptistebriel/biggie.git folder-name`

`cd folder-name && npm i && gulp`

Your site will be at `http://localhost:3000` by default using [browser-sync](http://www.browsersync.io)

## Gulp tasks

- `less` compilation to `css`
- browserify + babelify & uglify `js` files
  - use `build/app.js` for development, `build/app.min.js` for production
- watch for `css` and `js` files, livereload with browser-sync

## Todo

- [x] biggie + [wordpress](https://wordpress.org) *(will push to a new branch)*
- [x] biggie + [cockpit](http://getcockpit.com) *(will push to a new branch)*

### JS utils

Under `/assets/js/utils.js` there's a couple of `utils` functions:

- css
  - `getRect(top, right, bottom, left)` returns the css rect string with clip values
- js
  - `arrayFrom(opt)` returns an array from an argument (usually a `NodeList`)
  - `clamp(min, value, max)` return a clamped value between min and max values
  - `scrollTop` return either `pageYOffset` or `document.documentElement||document.body.scrollTop`
- biggie
  - `getSlug(req)` return the section slug (i.e. `home`) from bighweel's `req` parameter
  - `createPage(req, slug)` create an `HTML element` and returns it
  - `loadPage(req, view, done)` used on all sections's `init` to create the page

### Examples

- [oursroux.com](http://oursroux.com)
- [flavinsky.com](http://flavinsky.com)
- [pierrelevaillant.me](http://pierrelevaillant.me)
- [alisharaf.com](http://alisharaf.com)
- [bbriel.me](http://bbriel.me)
- [bigwheel-framework/built-with-bigwheel](https://github.com/bigwheel-framework/built-with-bigwheel)
- & more to come!

### License

MIT, see [LICENSE.md](https://github.com/baptistebriel/biggie/blob/gh-pages/LICENSE).
