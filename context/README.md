## ```context.environment```

Exposes the following properties.

* **appPath:** Path to running Pressmatic.app
* **userHome:** Path to current user home directory
* **phpVersion:** Available PHP versions in Pressmatic
* **version:** Pressmatic version
* **dockerPath:** Path to Docker binary in Pressmatic.app
* **userDataPath:** Path to Pressmatic user data folder. On Mac OS X this defaults to ~/Library/Application Support/Pressmatic

## ```context.hooks```

## ```context.electron```

Exposes [Electron API](http://electron.atom.io/docs/api/). The available methods and classes will differ based on whether or not this is ran from the main process or renderer process.

With the Electron API you can create dialogs, open new windows, and more.

## ```context.fileSystem```

Exposes [fs-extra](https://www.npmjs.com/package/fs-extra) NPM package which ends the native [fs API](https://nodejs.org/api/fs.html) in Node.js.

## ```context.fileSystemJetpack```

Exposes the [fs-jetpack](https://www.npmjs.com/package/fs-jetpack) NPM package. Some may prefer it over the native [fs API](https://nodejs.org/api/fs.html) in Node.js.

## ```context.notifier```

Exposes [node-notifier](https://www.npmjs.com/package/node-notifier) NPM package. The main method in this class is ```notify```.

#### Example

```js
context.notifier.notify({
  title: 'Notification Title',
  message: 'This is an example notification message.'
});
```

## ```context.process```
Exposes Node.js [process](https://nodejs.org/api/process.html) object.

## ```context.jQuery```
**Renderer Only**

```context.jQuery``` exposes [jQuery](http://api.jquery.com/) 2.2.3.

## ```context.React```
**Renderer Only**

```context.React``` to required to use JSX in your renderer entry point. You can also use context.React to access React's [Top-Level API](http://facebook.github.io/react/docs/top-level-api.html).

For more information about React in Pressmatic addons please see [Using React.js](references/using_reactjs.md).

## ```context.docker```