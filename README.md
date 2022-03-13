# eslint-config-mdh-typescript-react

Eslint config for TypeScript React🏄🏻

## Usage

After installation, make sure to remove all the eslint and prettier related dependencies.

Add `eslint-config-mdh-typescript-react` as part of `extends` in `.eslintrc.js` after installing the module.

```js
module.exports = {
  ...
  extends: ['eslint-config-mdh-typescript-react'],
  ...
};
```

To use prettier, add `"prettier": "eslint-config-mdh-typescript-react/prettier"` to `package.json`.
