# ajv-locale-code

Adds a `locale_code` format to [Ajv](https://ajv.js.org).

## Install

```bash
npm i --save @socketkit/ajv-locale-code
```

## Setup

```javascript
import Ajv from 'ajv'
import localeCode from '@socketkit/ajv-locale-code'
const ajv = new Ajv()
localeCode(ajv)
```

## Usage

When defining your JSON schema, use the `format` keyword with ther value set to `locale_code`. For example

```json
{
  "type": "object",
  "properties": {
    "locale": {
      "type": "string",
      "format": "locale_code"
    }
  }
}
```
