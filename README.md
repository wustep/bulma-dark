# @wustep/bulma-dark

![Safari screenshot](.github/safari-screenshot.png)

A [Bulma](https://bulma.io) extension that adds dark mode support via either the `prefers-color-scheme: dark` media query or a root class change. This is a fork of [`bulma-prefers-dark`](https://github.com/jloh/bulma-prefers-dark) that adds alternative sass files to import that support using classes as opposed to only the `prefers-color-scheme` tag.

Dark mode should be controlled, not assumed. This module lets the user control dark mode, optionally using their browser/OS preset as a default. [See this article for more details](https://piccalil.li/tutorial/create-a-user-controlled-dark-or-light-mode/).

## Installation

```
npm install wustep/bulma-dark
... Or ...
yarn add bulma-dark
```

## Usage

This extension works as-is in combination with Bulma! There are three different schemes to use this.

### bulma-prefers-dark

Add `bulma-prefers-dark.sass` for a dark themes that applies when the user has their `prefers-color-scheme` set to `dark`.

```scss
@import "../../node_modules/bulma/bulma.sass";
@import "../../bulma-prefers-dark/bulma-prefers-dark.sass";
```

or

```
@import '~bulma';
@import '~bulma-prefers-dark/bulma-prefers-dark.sass';
```

### bulma-dark-root

Add `bulma-dark-root.sass` instead for a dark theme that applies when the `<html>` tag has `class: dark-mode`.

### bulma-prefers-dark-root

Add `bulma-dark-and-prefers.sass` instead for a dark theme that applies when the `<html>` tag has `class: dark-mode` OR (`prefers-color-scheme` is set to `dark` AND the `<html>` tag does NOT have `class: light-mode`).

#### If using pure CSS without SASS

Note that the `/build/` and `/css` directories use the first: bulma-prefers-dark method! To change this, you can change the `@import "../bulma-prefers-dark.sass"` statement in `/build/bulma-prefers-dark.sass` and then run `npm build` to re-compile.

## Copyright & License

Original Code copyright 2019 James Loh. Code released under the [MIT license](LICENSE).
