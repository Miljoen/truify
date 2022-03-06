# Truify [![npm version](https://badgen.net/npm/v/truify?label=npm%20package&color=green&cache=600)][npm]

Simple package that truifies any input, except when it doesn't.

For more information, you are kindly referred to the Examples section.

## Technology
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

## Quick links
- Consult [CHANGELOG.md][changelog] for the project history.
- View [package repository][project] on GitHub.

## Installation

```
npm install truify
```

## Examples

```typescript
import { truify } from 'truify' // Supports ESM imports

truify(true) // true
truify(1) // true
truify(0.1) // true
truify(10) // true
truify(-1) // true
truify('String') // true
truify({}) // true
truify([]) // true

truify(false) // false
truify(0) // false
truify(null) // false
truify(NaN) // false
truify('') // false

truify() // Error!
```

## Contributors

View the full list of [contributors].

[npm]: https://www.npmjs.com/package/truify
[changelog]: https://github.com/Miljoen/truify/blob/master/CHANGELOG.md
[project]: https://github.com/Miljoen/truify
[contributors]: https://github.com/Miljoen/truify/graphs/contributors
