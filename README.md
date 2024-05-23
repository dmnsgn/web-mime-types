# web-mime-types

[![npm version](https://img.shields.io/npm/v/web-mime-types)](https://www.npmjs.com/package/web-mime-types)
[![stability-stable](https://img.shields.io/badge/stability-stable-green.svg)](https://www.npmjs.com/package/web-mime-types)
[![npm minzipped size](https://img.shields.io/bundlephobia/minzip/web-mime-types)](https://bundlephobia.com/package/web-mime-types)
[![dependencies](https://img.shields.io/librariesio/release/npm/web-mime-types)](https://github.com/dmnsgn/web-mime-types/blob/main/package.json)
[![types](https://img.shields.io/npm/types/web-mime-types)](https://github.com/microsoft/TypeScript)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-fa6673.svg)](https://conventionalcommits.org)
[![styled with prettier](https://img.shields.io/badge/styled_with-Prettier-f8bc45.svg?logo=prettier)](https://github.com/prettier/prettier)
[![linted with eslint](https://img.shields.io/badge/linted_with-ES_Lint-4B32C3.svg?logo=eslint)](https://github.com/eslint/eslint)
[![license](https://img.shields.io/github/license/dmnsgn/web-mime-types)](https://github.com/dmnsgn/web-mime-types/blob/main/LICENSE.md)

Mapping of the most common MIME types on the Web by extension. Currently 75 extensions.

[![paypal](https://img.shields.io/badge/donate-paypal-informational?logo=paypal)](https://paypal.me/dmnsgn)
[![coinbase](https://img.shields.io/badge/donate-coinbase-informational?logo=coinbase)](https://commerce.coinbase.com/checkout/56cbdf28-e323-48d8-9c98-7019e72c97f3)
[![twitter](https://img.shields.io/twitter/follow/dmnsgn?style=social)](https://twitter.com/dmnsgn)

## Installation

```bash
npm install web-mime-types
```

## Usage

```js
import webMimeTypes from "web-mime-types";

const jpegData = await (await fetch(url)).arrayBuffer();

const image = document.createElement("image");
image.src = URL.createObjectURL(
  new Blob([jpegData], { type: webMimeTypes["jpg"] }),
);
```

## API

<!-- api-start -->

<a name="module_web-mime-types"></a>

## web-mime-types

<a name="exp_module_web-mime-types--MIMETypesByExtension"></a>

### MIMETypesByExtension : <code>Object.&lt;string, MIMEType&gt;</code> ⏏

Map of file extension to MIME type

**Kind**: Exported constant
**See**: [MDN Common MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types)

<!-- api-end -->

## License

MIT. See [license file](https://github.com/dmnsgn/web-mime-types/blob/main/LICENSE.md).
