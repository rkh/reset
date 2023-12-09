# Yet another CSS reset

CSS/Sass reset based on [scss-reset](https://github.com/frontend-layers/scss-reset). Some rules specifically targeting very old browsers have been removed.

The main difference to other resets is that it wraps all resets rules in a CSS layer. This way they do not take precedence over your own CSS layers.

## Installation

With NPM:

```console
$ npm install --save @rkh/reset
```

With Yarn:

```console
$ yarn add @rkh/reset
```

## Usage

### Sass/SCSS

```scss
@use '@rkh/reset';
```

You may have to change the path depending on your setup.

It is also possible to use the reset without CSS layers:

```scss
@use '@rkh/reset' with ($use-layers: false);
```

Or with a custom layer name:

```scss
@use '@rkh/reset' with ($layer-name: 'my-reset-layer');
```

### CSS

```css
@import '@rkh/reset';
```

You may have to change the path depending on your setup.
