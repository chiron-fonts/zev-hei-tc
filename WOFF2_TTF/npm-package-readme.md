Zev Hei TC Webfont
======================

## About

This package contains the webfont version of [Zev Hei TC (宙黑體)](https://github.com/chiron-fonts/zev-hei-tc).

This package provides the webfont (WOFF2) build of the font. It utilizes Unicode-range subsetting technology to reduce
download size and improve loading performance. Check out the
project's [Github repository](https://github.com/chiron-fonts/zev-hei-tc) for a complete README (in Chinese only).

## Usage

To use this webfont, install the package first:

```bash
npm install zev-hei-tc-webfont 
```

Then, include either `css/zevheitc_n.css` file in your web page. For instance, if you use [webpack](https://webpack.js.org/), you
would import the font's CSS file with the following statement:

```css
// For the "N" variant:
@import '~zev-hei-tc-webfont/css/zevheitc_n.css';

// For the "F" variant:
@import '~zev-hei-tc-webfont/css/zevheitc_f.css';
```

Finally, set the `font-family` property to `ZevHeiTC-N Web` or `ZevHeiTC-F Web`:

```css
body {
    font-family: "ZevHeiTC-N Web", sans-serif;
}
```

You may use the `font-weight` CSS property to set the desired boldness. The following table shows the default static
font weights and their corresponding `font-weight` values. As a variable font, you may also specify any value between
200 and 900.

| Font Weight | CSS `font-weight` value |
|-------------|-------------------------|
| ExtraLight  | 200                     |
| Light       | 300                     |
| Normal      | 350                     |
| Regular     | 400                     |
| Medium      | 500                     |
| SemiBold    | 600                     |
| Bold        | 700                     |
| Heavy       | 900                     |

In addition, you can tweak the glyph space accommodation in the em-box via the font's "PADG" axis. For instance:

```css
p {
    font-variation-settings: "PADG" 6;
}
```

The PADG axis range is valid between 0 and 10. If unspecified, the default value is 0.”

## License

Zev Hei TC is licensed under the SIL Open Font License, Version 1.1. The full text of the license is available
at [https://openfontlicense.org/](https://openfontlicense.org/).
