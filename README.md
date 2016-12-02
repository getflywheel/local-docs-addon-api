# Local Add-on API

This guide is intended to get you up-and-running with the Local Add-on API. Local add-on's are written primarily in JavaScript and are modeled after Node.js packages.


## Structure

### [package.json](overview/addon_manifest.md)

The ```package.json``` file is a format for describing Node.js modules. Local add-ons are built on top of Node.js modules.

You must define a ```renderer``` and/or ```main``` entry-point.

### [Renderer Process Entry Point](overview/renderer_process.md)

The renderer process is what runs inside the main window. This is where you will add buttons, forms, and any other user interface elements.

Most add-ons will exclusively use the renderer process entry point for the sake of simplicity.

### [Main Process Entry Point](overview/main_process.md)

By tapping into the main process you can run processes even when the window is closed but Local is still running.

## Contribute To This Guide

You can contribute to improve this documentation on [GitHub](https://github.com/pressmatic/docs-addon-api) by opening issues or creating pull requests.
