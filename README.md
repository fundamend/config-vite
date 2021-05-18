# config-vite

_config-vite_ is a configuration preset for [Vite] used by the [fundamend.dev] ecosystem.

## Installation

Use your favorite Node.js package manager, for example [npm], like so:

    npm install --save-dev @fundamend/config-vite

... or [yarn], like so:

    yarn add --dev @fundamend/config-vite

## Usage

In your [vite.config.js], import _config-vite_ and spread it into the exported object, like so:

```js
const config = require('@fundamend/config-vite');

module.exports = {
	...config,
};
```

You can extend the imported preset by adding additional [configuration options] to the exported configuration object, for example like this:

```js
const config = require('@fundamend/config-vite');

module.exports = {
	...config,
	root: 'another/root',
};
```

Settings that already exist in the configuration preset will be overwritten.

## License

[MIT]

[configuration options]: https://vitejs.dev/config/#shared-options
[vite]: https://vitejs.dev/
[vite.config.js]: https://vitejs.dev/config/#config-file
[fundamend.dev]: https://fundamend.dev
[mit]: https://choosealicense.com/licenses/mit/
[npm]: https://www.npmjs.com/
[yarn]: https://yarnpkg.com/
