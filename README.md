# Pressmatic Addon API

This guide is intended to get you up-and-running with the Pressmatic Addon API. Pressmatic addon's are written primarily in JavaScript and are modeled after Node.js packages.


## Structure

### [package.json](overview/addon_manifest.md)

The ```package.json``` file is a format for describing Node.js modules. Pressmatic addons are built on top of Node.js modules.

You must define a ```renderer``` and/or ```main``` entry-point.

### [Renderer Process Entry Point](overview/renderer_process.md)

The renderer process is what runs inside the main window. This is where you will add buttons, forms, and any other user interface elements.

Most addons will exclusively use the renderer process entry point for the sake of simplicity.

### [Main Process Entry Point](overview/main_process.md)

By tapping into the main process you can run processes even when the window is closed but Pressmatic is still running.

## Contribute to this documentation

You can contribute to improve this documentation on [GitHub](https://github.com/pressmatic/docs-addon-api) by opening issues or creating pull requests.