# eslint-config-mdh-typescript-react

Eslint config for TypeScript React🏄🏻

## Usage

After installation, make sure to remove all the eslint and prettier related dependencies.

Add `eslint-config-mdh-typescript-react` as part of `extends` in `.eslintrc.js` after installing the module.

```js
module.exports = {
  root: true,
  env: {
    node: true,
  },
  extends: ['eslint-config-mdh-typescript-react'],
  parserOptions: {
    project: './tsconfig.json',
  },
  overrides: [{ files: ['**/*.ts'] }],
  rules: {},
}
```

To use prettier, add `"prettier": "eslint-config-mdh-typescript-react/prettier"` to `package.json`.

## Troubleshooting

If we are getting the error below, we can add the file into `.eslintignore`.

```
✖ eslint --ext js,jsx,ts,tsx --fix:

/../../../.eslintrc.js
  0:0  error  Parsing error: "parserOptions.project" has been set for @typescript-eslint/parser.
The file does not match your project config: .eslintrc.js.
The file must be included in at least one of the projects provided
```
