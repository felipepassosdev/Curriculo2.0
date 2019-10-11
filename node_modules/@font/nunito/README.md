# Nunito

Use the [Nunito Google Font](https://www.google.com/fonts/specimen/Nunito#charset) with your css pre-processor.

> Nunito is a well balanced Sans Serif with rounded terminals. Nunito has been designed mainly to be used as a display font but is usable as a text font too. Nunito has been designed to be used freely across the Internet by web browsers on desktop computers, laptops and mobile devices.

It is similar to the popular [Avenir](http://www.fonts.com/font/linotype/avenir).

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [Install](#install)
- [Usage](#usage)
- [Variables](#variables)
- [Developing](#developing)
  - [Requirements](#requirements)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Install

```sh
npm i -S @font/nunito
```

You'll also want a css-preprocessor that is capable of inlining `@import` statements and using CSS4 variable syntax. [atomify](htttp://github.com/atomify), [rework](https://github.com/reworkcss/rework), and [postcss](https://github.com/postcss/postcss) are all good choices.

## Usage

```css
@import "@font/nunito";

body {
  font-family: var(--fontFamily-nunito);
}

/* or get specific weights only */
@import "@font/nuninto/regular";

body {
  font-family: var(--fontFamily-nunito);
  font-weight: var(--fontWeight-nunito-regular);
}
```

## Variables
```css
:root {
  --fontWeight-nunito-light: 300;
  --fontWeight-nunito-regular: 400;
  --fontWeight-nunito-bold: 700;
  --fontFamily-nunito: 'Nunito', sans-serif;
}
```

## Developing
To publish, run `npm run release -- [{patch,minor,major}]`

_NOTE: you might need to `sudo ln -s /usr/local/bin/node /usr/bin/node` to ensure node is in your path for the git hooks to work_

### Requirements
* **npm > 2.0.0** So that passing args to a npm script will work. `npm i -g npm`
* **git > 1.8.3** So that `git push --follow-tags` will work. `brew install git`

## License

Artistic 2.0 © [Joey Baker](https://byjoeybaker.com)


[npm-url]: https://npmjs.org/package/@font/nunito
[npm-image]: https://badge.fury.io/js/@font/nunito.svg
[travis-url]: https://travis-ci.org/joeybaker/@font/nunito
[travis-image]: https://travis-ci.org/joeybaker/@font/nunito.svg?branch=master
[daviddm-url]: https://david-dm.org/joeybaker/@font/nunito.svg?theme=shields.io
[daviddm-image]: https://david-dm.org/joeybaker/@font/nunito
