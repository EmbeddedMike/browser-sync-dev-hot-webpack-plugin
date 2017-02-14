# browser-sync-dev-hot-webpack-plugin

[![Greenkeeper badge](https://badges.greenkeeper.io/itgalaxy/browser-sync-dev-hot-webpack-plugin.svg)](https://greenkeeper.io/)

Combines BrowserSync, webpack-dev-middleware, and webpack-hot-middleware into one plugin.

## Install

```shell
npm install --save-dev browser-sync-dev-hot-webpack-plugin
```

## Usage

```js
const BROWSER_SYNC_OPTIONS = {};
const DEV_MIDDLEWARE_OPTIONS = {
    publicPath: '/my/public/path'
};
const HOT_MIDDLEWARE_OPTIONS = {};

const webpackConfig = {
    // Some options...
    plugins: [
        // Other plugins...
        new BrowserSyncHotPlugin({
            browserSyncOptions: BROWSER_SYNC_OPTIONS,
            devMiddlewareOptions: DEV_MIDDLEWARE_OPTIONS,
            hotMiddlewareOptions: HOT_MIDDLEWARE_OPTIONS,
            callback() {
                console.log('Callback')
            }
        })
        // Other plugins...
    ]
    // Some options...
};

module.exports = webpackConfig;
```

## Options

See related packages docs.

## Related

- [browser-sync](https://github.com/browsersync/browser-sync) - Keep multiple browsers & devices 
in sync when building websites.

- [webpack-dev-middleware](https://github.com/webpack/webpack-dev-middleware) - Offers a dev middleware for webpack, 
which arguments a live bundle to a directory.

- [webpack-hot-middleware](https://github.com/glenjamin/webpack-hot-middleware) - Webpack hot reloading 
you can attach to your own server.

## Contribution

Feel free to push your code if you agree with publishing under the MIT license.

## [Changelog](CHANGELOG.md)

## [License](LICENSE)
