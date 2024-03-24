# tsconfig-jsdoc

This package contains `tsconfig.json` files for use with [JSDoc types](https://www.typescriptlang.org/docs/handbook/jsdoc-supported-types.html) in modern javascript runtimes.

Our approach is to set everything as strictly as possible for consumers to opt out rather than opt in for correctness checks. We do not enable stylistic settings by default.

## Usage
### Install

#### npm
```
npm i -D tsconfig-jsdoc
```

#### pnpm
```
pnpm i -D tsconfig-jsdoc
```

#### yarn
```
yarn add tsconfig-jsdoc --dev
```

### tsconfig.json
#### Browsers
```
{
    "extends": ["tsconfig-jsdoc/tsconfig.browser.json"],
    "include": ["src/**/*.js"]
}
```
#### Cloudflare
```
{
    "extends": ["tsconfig-jsdoc/tsconfig.cloudflare.json"],
    "include": ["src/**/*.js"]
}
```
#### Other
#### Browsers
```
{
    "extends": ["tsconfig-jsdoc/tsconfig.json"],
    "include": ["src/**/*.js"]
}
```