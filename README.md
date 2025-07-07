# Electron Auto-Updater Demo

This Electron app opens [google.com](https://www.google.com) and includes auto-update functionality using `electron-updater`.

## Getting Started

### Install dependencies
```sh
npm install
```

### Run the app
```sh
npm start
```

### Build the app
```sh
npm run dist
```
The build output will be in the `dist/` directory.

## Auto-Update Setup

- The app is configured to use a generic update server. Update the `url` in the `publish` section of `package.json` to point to your update server.
- To publish updates:
  1. Build a new version (increment the version in `package.json`).
  2. Upload the generated files in `dist/` (including `.yml` and installer) to your update server.
  3. The app will check for updates on launch and notify the user if an update is available.

## Notes
- For production, you must set up a real update server and use HTTPS.
- See [electron-builder docs](https://www.electron.build/auto-update) for more details on auto-update configuration. 