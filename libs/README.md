# LIBRARY CODE

The main file in this directory is `addAccessibilityRules.js`, whose default export is re-exported from `src/index.js`.  This is the only publicly accessible function thus far.

All other files exist as supplementary code for this function, and serve as helpful abstractions when the code outgrows the scope of its concerns.  As a general rule, these other files are named after their default export, which are *usually* functions.

Breaking every piece down in a functional way makes the code more testable.

## Development Server

For practical testing purposes, there is a `demo/` folder at the root directory which contains HTML, JS, and CSS that run on a simple Express server via `demoServer.js` which is also located at the root, on `localhost:3000`.
```
npm start
```

## Build Process

This project uses Rollup to bundle all source code into all kinds of modules, including ESM, CMD, and UMD.  These configurations can be found in `rollup.config.js` located in the root directory.
```
npm run build
```
