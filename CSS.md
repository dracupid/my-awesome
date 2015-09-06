## CSS
- [CSS Guildelines](http://cssguidelin.es/): by Harry Roberts
- [Block Element Modifier](http://getbem.com/): A methodology to achieve reusable components and code sharing in the front-end.

#### libs
- [normalize.css](https://github.com/necolas/normalize.css/): A customisable CSS file that makes browsers render all elements more consistently and in line with modern standards
    + [Prefer normalize to traditional Reset](http://nicolasgallagher.com/about-normalize-css/)
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
    + [est](https://github.com/ecomfe/est): Less mixins.<iframe src="https://ghbtns.com/github-btn.html?user=ecomfe&repo=est&type=star&count=true" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>
    + <del>[LESS Hat](https://github.com/madebysource/lesshat): Less mixins.[outdated]<del><iframe src="https://ghbtns.com/github-btn.html?user=madebysource&repo=lesshat&type=star&count=true" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>

### [Stylus](http://learnboost.github.io/stylus/)
- library
    - [nib](https://github.com/tj/nib): Stylus mixins, utilities, components, and gradient image generation <iframe src="https://ghbtns.com/github-btn.html?user=tj&repo=nib&type=star&count=true" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>

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
    + ** Don't use anything but Autoprefixer to add vendor prefixes.**
- [CSS Grace][]: Handles IE hacks (opacity, rgba, inline-block, etc) in addition to some non-standard handy shortcuts.
- [rucksack][]: A little bag of CSS superpowers
- [cssnext][]: Use tomorrow's CSS syntax, today. (Includes autoprefixer)
- [...](https://github.com/postcss/postcss#plugins)

#### minify
[benchmark](https://github.com/GoalSmashers/css-minification-benchmark)

<del>[rework](https://github.com/reworkcss/rework): CSS manipulations built on [css](https://github.com/reworkcss/css). [out of fashion]</del>

[Autoprefixer]: https://github.com/postcss/autoprefixer
[CSS Grace]: https://github.com/cssdream/cssgrace
[cssnext]: https://github.com/cssnext/cssnext
[clean-css]: https://github.com/jakubpawlowicz/clean-css
[PostCSS]: https://github.com/postcss/postcss
[rucksack]: https://github.com/simplaio/rucksack
