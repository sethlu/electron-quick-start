# electron-quick-start

This fork presents a reproduction of issue [electron-osx-sign#155](https://github.com/electron-userland/electron-osx-sign/issues/155) that results in failure to code sign apps on macOS High Sierra (only tested platform).

There are three related scripts to this demo; before running, ensure that a `Mac Developer` certificate is installed in the system default keychain and that a development provisioning profile is placed in the current working directory for `electron-osx-sign` to pick up.

- `npm run package-test`

  To ensure that by default the app could function after codesigned with App Sandbox enabled, this command packages and signs a demo application that should be able to run with ease.

- `npm run package-test-fail`

  App packaging should work, but codesigning should fail.

- `npm run package-test-succeed`

  App packaging and codesigning should both succeed.

More discussions related to this issue should be found on [electron-osx-sign#155](https://github.com/electron-userland/electron-osx-sign/issues/155).

## To Use

To clone and run this repository you'll need [Git](https://git-scm.com) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/electron/electron-quick-start
# Go into the repository
cd electron-quick-start
# Install dependencies
npm install
```

Learn more about Electron and its API in the [documentation](http://electron.atom.io/docs/latest).

#### License [CC0 (Public Domain)](LICENSE.md)
