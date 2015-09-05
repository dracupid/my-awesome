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

> In my opinion, a CSS preprocessor, including their libraries should not do or use a plugin/middleware system  to achive follow functions:
> - Add vendor prefixes. Things should change after autoprefixer was born.
> - Any process after CSS is generated. Such as minify.
> - Anything beyond string to string transforming.

## preprocessor
[PostCSS][]: Transforming CSS with JS plugins
- [Autoprefixer][]: Add vendor prefixes using values from Can I Use. [Try online](http://simevidas.jsbin.com/gufoko/quiet)
- [CSS Grace][]: Handles IE hacks (opacity, rgba, inline-block, etc) in addition to some non-standard handy shortcuts.
- [cssnext][]: Use tomorrow's CSS syntax, today. (Includes autoprefixer)
- [...](https://github.com/postcss/postcss#plugins)

<del>[rework](https://github.com/reworkcss/rework): CSS manipulations built on [css](https://github.com/reworkcss/css). [out of fashion]</del>

> Actually PostCss is not only a postprocessor. It can do nearly everything a preprocessor or its library can. The mainly difference is that a preprocessor is more like a template language where you can mix styles with code. With postprocessor you are writing a customized CSS.

> 目前的情况是，preprocessor和preprocessor的功能有较多的重合之处，预处理和后处理的分界很不明确，二者都想独揽CSS工具链，产生了很多做越界工作的插件。我认为，CSS的工具链中，预处理和后处理的界限应该明确。

> preprocessor，主要形式是CSS预编译语言，其产生的是符合CSS标准语法的CSS文件。功能主要应限于以下几点：
> - 提供更简便清晰的样式表书写语法，提升CSS的生产效率。
> - 在语法层面扩充CSS语言特性。如变量, mixin, nesting，模块化等等。Postcss中涉及自定义语法的内容应该由preprocessor完成。
> - 在条件允许的情况下增加对下一代CSS标准语法的支持。（注意是语法，而不是CSS属性，参考[cssnext](http://cssnext.io/features/)）

> postprocessor的输入和输出都是符合CSS标准语法的CSS文件，其功能应限于以下几点
> - 只做CSS属性的添改，不在语法层面对CSS进行扩充。
> - 可以使用某些特殊的属性或属性值用作标识，在处理后替换为有效的值。以此支持一些常用helper.
> - 修正浏览器兼容性问题和常见错误，使得开发者不需要为此多虑。如浏览器前缀, bug fix 和 IE HACK。如[Autoprefixer][], [CSS Grace][]
> - 精简和清理CSS中的冗余内容。如[css-nano](https://github.com/ben-eb/cssnano)

> 一般来讲，preprocessor是排他的，而postprocessor可以按照一定的顺序结合使用。当然，preprocessor和postprocessor的工作可以由一个框架完成，比如[PostCSS][]，但是二者在工具链中的位置和职能应该明确。从现在开始，在开发过程中，我也建议按照之前的划分来选择和部署工具。

> 此外，在CSS工具链的末端还有CSS的minify工具，如[clean-css][]

[Autoprefixer]: https://github.com/postcss/autoprefixer
[CSS Grace]: https://github.com/cssdream/cssgrace
[cssnext]: https://github.com/cssnext/cssnext
[clean-css]: https://github.com/jakubpawlowicz/clean-css
[PostCSS]: https://github.com/postcss/postcss
