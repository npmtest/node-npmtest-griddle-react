# npmtest-griddle-react

#### basic test coverage for  griddle-react (v1.3.1)  [![npm package](https://img.shields.io/npm/v/npmtest-griddle-react.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-griddle-react) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-griddle-react.svg)](https://travis-ci.org/npmtest/node-npmtest-griddle-react)

#### A fast and flexible grid component for React

[![NPM](https://nodei.co/npm/griddle-react.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/griddle-react)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-griddle-react/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-griddle-react/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-griddle-react/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-griddle-react/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-griddle-react/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-griddle-react/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-griddle-react/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-griddle-react/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-griddle-react/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-griddle-react/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-griddle-react/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-griddle-react/build/test-report.html](https://npmtest.github.io/node-npmtest-griddle-react/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-griddle-react/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-griddle-react/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-griddle-react/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-griddle-react/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-griddle-react/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-griddle-react/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-griddle-react/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-griddle-react/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ryan Lanciaux & Joel Lanciaux"
    },
    "ava": {
        "require": [
            "babel-register"
        ],
        "babel": "inherit"
    },
    "dependencies": {
        "immutable": "^3.8.1",
        "lodash": "^4.17.4",
        "max-safe-integer": "^1.0.0",
        "react-redux": "^5.0.2",
        "recompose": "^0.21.2",
        "redux": "^3.5.2",
        "reselect": "^2.5.3"
    },
    "description": "A fast and flexible grid component for React",
    "devDependencies": {
        "@kadira/storybook": "^2.5.2",
        "@types/react": "^15.0.17",
        "ava": "^0.17.0",
        "babel-cli": "^6.23.0",
        "babel-core": "^6.0.0",
        "babel-loader": "^6.0.0",
        "babel-plugin-lodash": "^3.2.11",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-react": "^6.5.0",
        "babel-preset-stage-0": "^6.0.0",
        "babel-register": "^6.9.0",
        "cross-env": "^3.2.4",
        "enzyme": "^2.7.1",
        "eslint": "^3.9.1",
        "eslint-config-airbnb": "^14.0.0",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-jsx-a11y": "^3.0.2",
        "eslint-plugin-react": "^6.6.0",
        "jsdom": "^9.10.0",
        "jsdom-global": "^2.1.1",
        "lodash-webpack-plugin": "^0.11.0",
        "node-libs-browser": "^2.0.0",
        "react": "^15.3.2",
        "react-addons-test-utils": "^15.0.1",
        "react-dom": "^15.3.2",
        "rimraf": "^2.6.0",
        "ts-loader": "^2.0.2",
        "typescript": "^2.2.1",
        "webpack": "^1.14.0",
        "webpack-dev-server": "^1.16.2"
    },
    "directories": {},
    "dist": {
        "shasum": "efcbfb8e51fe596de9e8d292622f9cc8744faa24",
        "tarball": "https://registry.npmjs.org/griddle-react/-/griddle-react-1.3.1.tgz"
    },
    "gitHead": "8bd116cb505c25de1417d1da847dc3df44cdec6a",
    "keywords": [
        "react-component",
        "grid",
        "react",
        "pagination",
        "sort"
    ],
    "license": "MIT",
    "main": "dist/module/module.js",
    "maintainers": [
        {
            "name": "joellanciaux"
        },
        {
            "name": "kevinold"
        },
        {
            "name": "ryanlanciaux"
        }
    ],
    "name": "griddle-react",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": ">=15"
    },
    "scripts": {
        "build": "npm run clean-dist && npm run build-modules && npm run build-umd && npm run build-ts",
        "build-modules": "cross-env BABEL_ENV=build babel src --out-dir dist/module ",
        "build-storybook": "build-storybook",
        "build-ts": "cp src/module.d.ts dist/module/",
        "build-umd": "webpack --config webpack.config.js",
        "clean-dist": "rimraf dist",
        "ship-it": "npm run build && npm publish --tag next",
        "start": "start-storybook -p 6006",
        "storybook": "start-storybook -p 6006",
        "test": "ava",
        "watch-test": "ava --watch"
    },
    "types": "dist/module/module.d.ts",
    "version": "1.3.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
