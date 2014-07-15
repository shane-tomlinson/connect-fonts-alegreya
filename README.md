# connect-fonts-alegreya

Alegreya fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-alegreya");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/alegreya-black/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/alegreya-black,alegreya-blackitalic,alegreya-bold,alegreya-bolditalic,alegreya-italic,alegreya-regular/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* alegreya-black
* alegreya-blackitalic
* alegreya-bold
* alegreya-bolditalic
* alegreya-italic
* alegreya-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/alegreya-black/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin

5. Set your CSS up to use the new font by using the "Alegreya" font-family.
```
    body {
      font-family: 'Alegreya', 'sans-serif', 'serif';
    }
```

## Font Info
Alegreya

* Copyright: Copyright (c) 2011, Juan Pablo del Peral (juan@huertatipografica.com.ar), with Reserved Font Names "Alegreya" "Alegreya SC"
* Trademark: Alegreya is a trademark of Juan Pablo del Peral
* Designer: Juan Pablo del Peral
* Designer URL: www.huertatipografica.com.ar 
* Vendor: Juan Pablo del Peral
* Vendor URL: www.huertatipografica.com.ar

## Development Info

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 1.1 of the SIL Open Font License

  http://scripts.sil.org/OFL

