# cabin.sass
> Some common [Sass][] helpers we use across projects.

[Sass]: http://sass-lang.com/

Install via bower:

    % bower install --save https://github.com/cabin/cabin.sass.git

## cabin-defaults($selector: null)
Include this mixin at the top level to apply baseline house styles. To limit
its effects to a wrapper element, pass a selector argument.

## prevent-tap-highlight
Hide Mobile Safari's background flash on tap.

## reduce-font-dilation($value: true)
Switch from subpixel antialiasing to greyscale, which reduces artificially-
inflated font weight on Mac OS X. Particularly useful with light-on-dark text
or with `@font-face`d web fonts.
See <http://lists.w3.org/Archives/Public/www-style/2012Oct/0109.html>.

## voffset($height, $offset: null)
Elements with all-uppercase text appear off-center visually due to unused
descender space. This allows for shifting them down a bit. If called with only
one argument, it is used as `$offset` (despite the parameter order here).
