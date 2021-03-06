# sauna

> Sauna is an alternate client for Steam chat built on [Electron](https://electron.atom.io), using [node-steam-user](https://github.com/DoctorMcKay/node-steam-user) to interface with the desktop Steam API.

## Install

`steam-user` is not listed as an explicit dependency as it seems that installing it tends to fail when done automatically. Instead, to install, make you sure have `svn` in your path, then run the following commands inside the `sauna` folder:

```sh
npm install
npm install steam-user
npm install steam
cd node_modules/steam
npm install steam-resources
cd node_modules/steam-resources
npm install
cd ../../../..
```

On Windows, you may need to add `--no-bin-links` to `npm install steam-user` and `npm install steam-resources`.

To run `sauna` from source, you need to have the `electron` binary. Install `electron-prebuilt` globally, then run it:

```sh
npm install -g electron-prebuilt
electron . # where . is the path to the `sauna` folder
```
