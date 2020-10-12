# svelte-bootstrap-icons

[![NPM][npm]][npm-url]
[![Build][build]][build-badge]

> [Bootstrap SVG icons](https://github.com/twbs/icons) as Svelte components.

Try it in the [Svelte REPL](https://svelte.dev/repl/9a0e245df66248d59fadbbf007c06124?version=3.24.0).

## [Icon Preview](https://metonym.github.io/svelte-bootstrap-icons/)

## Install

This library requires Svelte version >=3.20 because it uses `$$restProps`.

```sh
yarn add -D svelte-bootstrap-icons
# OR
npm i -D svelte-bootstrap-icons
```

## Usage

```html
<script>
  import Alarm from "svelte-bootstrap-icons/lib/Alarm";
</script>

<Alarm />
```

Refer to [ICON_INDEX.md](ICON_INDEX.md) for list of icons.

## API

`$$restProps` are forwarded to the `svg` element.

### Forwarded events

- on:click
- on:mouseover
- on:mouseenter
- on:mouseout
- on:keydown

## [Changelog](CHANGELOG.md)

## Development workflow

Svelte components are generated from "bootstrap-icons" SVG files using [svg-to-svelte](https://github.com/metonym/svg-to-svelte).

A single script ([build.js](build.js)) specifies the input and output folders.

The generated Svelte components are located in the `lib` folder, which is ignored by Git but published to NPM.

Documentation is generated using the list of icon module names from the source library (see [ICON_INDEX.md](ICON_INDEX.md)).

## License

[MIT](LICENSE)

[npm]: https://img.shields.io/npm/v/svelte-bootstrap-icons.svg?color=blue
[npm-url]: https://npmjs.com/package/svelte-bootstrap-icons
[build]: https://travis-ci.com/metonym/svelte-bootstrap-icons.svg?branch=master
[build-badge]: https://travis-ci.com/metonym/svelte-bootstrap-icons
