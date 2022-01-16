# @jessety/prettier-config

Yet another Prettier [shareable config](https://prettier.io/docs/en/configuration.html#sharing-configurations).

[![ci](https://github.com/jessety/prettier-config/workflows/ci/badge.svg)](https://github.com/jessety/prettier-config/actions/workflows/ci.yml)
[![npm](https://img.shields.io/npm/v/@jessety/prettier-config.svg)](https://www.npmjs.com/package/@jessety/prettier-config)
[![license](https://img.shields.io/github/license/jessety/prettier-config.svg)](https://github.com/jessety/prettier-config/blob/main/LICENSE)

## Installation

```shell script
npm i -D prettier @jessety/prettier-config
```

## Usage

Reference this package in the `prettier` section of your `package.json`:

```json
{
  "name": "your-package-name",
  "version": "1.0.0",
  "prettier": "@jessety/prettier-config"
}
```

Alternatively, export a string to that references this package from your `prettier` config file.

For example, a valid `.prettierrc.json` file would be:

```json
"@jessety/prettier-config"
```

## Extending

To extend this config file in your project, use a `.prettierrc.js` file:

```javascript
module.exports = {
  ...require('@jessety/prettier-config'),
  printWidth: 100,
};
```

## License

MIT © Jesse Youngblood
