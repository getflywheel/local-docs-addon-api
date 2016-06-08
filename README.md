# Addon API

This guide is intended to get you up-and-running with the Pressmatic Addon API. Pressmatic addon's are written primarily in JavaScript and are modeled after Node.js packages.


## Structure


### [package.json](addon_manifest.md)


The ```package.json``` file is a format for describing Node.js modules. Pressmatic addons are built on top of Node.js modules.

You must define ```main``` and/or ```renderer``` entry-points.

### Main Process Entry Point

### Renderer Process Entry Point