# VueCountryFlagTest (vuecountryflagtest)

Test env for catching VueCountryFlag plugin issue

## Install the dependencies
```bash
npm install
cd src-cordova
npm install
cordova platform add android
```

### Start the app in development mode (hot-code reloading, error reporting, etc.)
```bash
quasar dev
```

### NB! Build an android-version of this application (Get app-debug-unsigned.apk or app-debug.apk file, you can install it on your phone or run in android-emulator)
```bash
quasar build -m cordova -T android
```

OR

```bash
quasar build -m cordova -T android
cd src-cordova
cordova build android
```

### Lint the files
```bash
npm run lint
```

### Build the app for production
```bash
quasar build
```
