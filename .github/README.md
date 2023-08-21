# NPM Package Project Template

## About the Project

A package template for building your npm packages/libraries with the latest dependencies. This template uses [Rollup](https://www.npmjs.com/package/rollup) as the bundler.


## Prerequisites

1. [Node Package Manager (npm)](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
1. [Node Version Manager (nvm)](https://css-tricks.com/how-to-install-npm-node-nvm/)
1. [Yarn](https://classic.yarnpkg.com/lang/en/docs/install)

## How to Set up

1. Clone and rename this repository into your local

1. Go to project root directory and install

   ```bash
   cd rma-npm-package-template
   nvm install
   yarn install
   ```

1. Create your first function. Or just use the existing for now.

1. Make some changes to `package.json`
   - `author` - ofcourse, you 😊
   - `name` - package name that will appear in NPM

1. Build it
   ```bash
   yarn build
   ```

   > In the root directory, you will see `dist` folder with 5 files:
   > `index.cjs.js` (commonjs format)
   > `index.d.ts` (typescript declaration)
   > `index.es.js` (es format)
   > `index.js` (iife format)
   > `index.min.js` (iife minified format)
   >
   > You can limit the output formats in `rollup.config.js`

1. In the same terminal and directory, login to your npm account. Then, publish

   ```bash
   npm version <new version>
   npm publish
   ```
