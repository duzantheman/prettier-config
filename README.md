# prettier-config
My central Prettier config file

## Install

```
npm i -D @cgduzan/prettier-config prettier @trivago/prettier-plugin-sort-imports
```

## Usage

Create or update a `.prettierrc.js` file with the following format:

```
module.exports = {
  ...require("@cgduzan/prettier-config"),

  // include this if there is a particular import order
  // importOrder: [],
}
```

or in your `package.json` (if not specifying `importOrder`):

```
{
  "prettier": "@cgduzan/prettier-config"
}
```

If using the `.prettierrc.js` file and a `.prettierrc` file currently exists, be sure to remove the `.prettierrc` file and update any `prettier` npm scripts to point at the new `.prettierrc.js` file

## Rules

Here are the [Prettier options](https://prettier.io/docs/en/options.html) and the [prettier-plugin-sort-imports options](https://github.com/trivago/prettier-plugin-sort-imports/blob/master/README.md)

(Almost) all options are included in this module, even if they are using the default value. That way, it is easier to see what options are available and change them if necessary.
