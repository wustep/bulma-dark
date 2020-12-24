# @wustep/bulma-dark

![Safari screenshot](.github/safari-screenshot.png)

A Bulma extension that adds support for the `prefers-color-scheme: dark` media query



## Installation

```
npm install wustep/bulma-dark
... Or ...
yarn add bulma-dark
```

## Usage 

This extension works as-is in combination with Bulma! There are two ways to use this.

### bulma-prefers-dark

Add `bulma-prefers-dark.sass` for themes that apply when the user has their `prefers-color-scheme` set to true.

```scss
@import "../../node_modules/bulma/bulma.sass";
@import "../../bulma-prefers-dark/bulma-prefers-dark.sass";
```

or 

```
@import '~bulma';
@import '~bulma-prefers-dark/bulma-prefers-dark.sass';
```

### bulma-dark

Add `bulma-dark.sass` for themes that apply when the `<html>` tag has `class: dark-mode`.

## Copyright & License

Code copyright 2019 James Loh. Code released under the [MIT license](LICENSE).
