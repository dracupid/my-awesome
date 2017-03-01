## CSS

- [CSS Guildelines](http://cssguidelin.es/): by Harry Roberts
- [Block Element Modifier](http://getbem.com/): A methodology to achieve reusable components and code sharing in the front-end.

#### uniform
- [normalize.css](https://github.com/necolas/normalize.css/): Render elements more consistently with each other.
    + [Prefer normalize to traditional Reset](http://nicolasgallagher.com/about-normalize-css/)
- [sanitize.css](https://github.com/10up/sanitize.css): Render elements more consistently with developer expectations and preferences.

#### libs
- [animate.css](https://github.com/daneden/animate.css): I'd like to use it only as a css `animate` reference.
- [Font Awesome](https://github.com/FortAwesome/Font-Awesome): Use icons as a single font.

## preprocessor
A preprocessor is mostly an extended CSS "language" or special syntax which allow you to write CSS gracefully and faster. It may have following features:
- variable and Interpolation
- mixin/extend
- function
- nesting
- operations
- condition and loop
- modularize(importing)

As far as I know, all preprocessors by now only extends CSS syntax, which means you can mix using pure CSS with any of them without any bother.

Less, stylus and Sass are the most popular three.
### [Less](http://lesscss.org/)
- library
    + [est](https://github.com/ecomfe/est): Less mixins.
    + <del>[LESS Hat](https://github.com/madebysource/lesshat): Less mixins.[outdated]<del>

### [Stylus](http://learnboost.github.io/stylus/)
- library
    - [nib](https://github.com/tj/nib): Stylus mixins, utilities, components, and gradient image generation

### [Sass / SCSS](http://sass-lang.com/)
- library
    - [Bourbon](https://github.com/thoughtbot/bourbon): A simple and lightweight mixin library for Sass.
    - [Compass](https://github.com/Compass/compass/): A CSS Authoring Framework
- style
    - [Sass Guidelines](http://sass-guidelin.es/) by Hugo Giraudel

Sass was originally written in Ruby.

## postprocessor
[PostCSS][]: Transforming CSS with JS plugins
- **[Autoprefixer][]**: Add vendor prefixes using values from Can I Use. [Try online](http://simevidas.jsbin.com/gufoko/quiet)
    + **Don't use anything but Autoprefixer to add vendor prefixes.**
- [CSS Grace][]: Handles IE hacks (opacity, rgba, inline-block, etc) in addition to some non-standard handy shortcuts.
- [rucksack][]: A little bag of CSS superpowers
- [cssnext][]: Use tomorrow's CSS syntax, today. (Includes autoprefixer)
- [...](https://github.com/postcss/postcss#plugins)

#### minify
- [benchmark](https://github.com/GoalSmashers/css-minification-benchmark): A comparison of CSS minifiers
- [clean-css][]: A fast, efficient, and well tested CSS minifier
- [cssnano][]: A modular minifier, built on top of the PostCSS ecosystem. But it's slow.

[Autoprefixer]: https://github.com/postcss/autoprefixer
[CSS Grace]: https://github.com/cssdream/cssgrace
[cssnext]: https://github.com/cssnext/cssnext
[clean-css]: https://github.com/jakubpawlowicz/clean-css
[PostCSS]: https://github.com/postcss/postcss
[rucksack]: https://github.com/simplaio/rucksack
[cssnano]: https://github.com/ben-eb/cssnano
