# ESLint config

## Whats included?

- Standard config base
- React plugin
- JSX a11y plugin
- Import helpers plugin
- Prettier

## Setup

Install the dependencies:

```bash
npm i -D eslint @sup3r-us3r/eslint-config
```

Create a `.eslintrc` file extending the config:

```json
{
  "extends": "@sup3r-us3r/eslint-config/react"
}
```

> You can also use a `.eslintrc.json` or `.eslintrc.js`.

Add `lint` script in your `package.json` to try fix all lint errors:

```json
"scripts": {
  "lint": "eslint \"src/**/*.{js,jsx,ts,tsx}\" --fix"
}
```

## Prettier config

Create `.prettierrc` file in the root directory with below content:

```json
{
  "semi": true,
  "singleQuote": true,
  "arrowParens": "avoid",
  "trailingComma": "all",
  "endOfLine": "lf"
}
```

Or copy this config:

```sh
$ cp node_modules/@sup3r-us3r/eslint-config/.prettierrc .
```

> Run the above command in your project root directory.

## Editor config

Create `.editorconfig` file in the root directory with below content:

```text
root = true

[*]
indent_style = space
indent_size = 2
end_of_line = lf
charset = utf-8
trim_trailing_whitespace = true
insert_final_newline = true
```

Or copy this config:

```sh
$ cp node_modules/@sup3r-us3r/eslint-config/.editorconfig .
```

> Run the above command in your project root directory.
