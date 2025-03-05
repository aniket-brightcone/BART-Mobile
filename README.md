# BART Mobile App

A mobile application for Bay Area Rapid Transit (BART) users that provides real-time information, trip planning, and station details.

## Features

- Real-time train arrivals and departures
- Station information and maps
- Trip planning with fare estimates
- Service advisories and alerts
- Saved favorite stations and routes

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18 or newer)
- [npm](https://www.npmjs.com/) (v9 or newer)
- [Git](https://git-scm.com/)
- [Expo CLI](https://docs.expo.dev/more/expo-cli/)

For iOS development:
- macOS
- [Xcode](https://developer.apple.com/xcode/) (latest version recommended)
- iOS Simulator

For Android development:
- [Android Studio](https://developer.android.com/studio)
- Android Emulator

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/aniket-brightcone/BART-mobile-app.git
   cd BART-Mobile
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Running the App

### Start the Development Server

```bash
npm start
# or
npx expo start
```

This will start the Expo development server and display a QR code and options for running the app.

### Run on iOS Simulator

1. Make sure you have Xcode installed with iOS Simulator.
2. Start the development server with:
   ```bash
   npm run ios
   # or
   npx expo start --ios
   ```
   This will automatically open the app in the iOS Simulator.

3. Alternatively, after starting the server with `npm start`, press `i` in the terminal to open in iOS Simulator.

### Run on Android Emulator

1. Make sure you have Android Studio installed with an Android Virtual Device (AVD).
2. Start your Android emulator from Android Studio or command line.
3. Start the development server with:
   ```bash
   npm run android
   # or
   npx expo start --android
   ```
   This will automatically open the app in the Android emulator.

4. Alternatively, after starting the server with `npm start`, press `a` in the terminal to open in Android emulator.

### Run on Physical Device

1. Install the Expo Go app on your [iOS](https://apps.apple.com/app/expo-go/id982107779) or [Android](https://play.google.com/store/apps/details?id=host.exp.exponent) device.
2. Start the development server with `npm start`.
3. Scan the QR code with your device:
   - iOS: Use the Camera app
   - Android: Use the Expo Go app

## Development Builds

For a more native experience and to test native modules:

1. Create a development build:
   ```bash
   npx expo prebuild
   ```

2. Run the development build:
   ```bash
   npx expo run:ios
   # or
   npx expo run:android
   ```

## Troubleshooting

### Common Issues

1. **Metro bundler not starting**
   - Try clearing the cache: `npx expo start --clear`

2. **iOS Simulator not opening**
   - Ensure Xcode is up to date
   - Try running: `xcrun simctl list devices` to see available simulators
   - Open Xcode and check for any pending updates or agreements

3. **Android Emulator issues**
   - Ensure your emulator is running before starting the app
   - Check that ANDROID_HOME environment variable is set correctly
   - Try creating a new AVD in Android Studio

4. **Dependencies issues**
   - Try removing node_modules and reinstalling: 
     ```bash
     rm -rf node_modules
     npm install
     ```

5. **Expo Go compatibility**
   - Some features may not work in Expo Go if they require native modules
   - Consider creating a development build for full functionality

### Getting Help

If you encounter any issues not covered here, please:
1. Check the [Expo documentation](https://docs.expo.dev/)
2. Visit the [Expo forums](https://forums.expo.dev/)
3. Search for similar issues on [Stack Overflow](https://stackoverflow.com/questions/tagged/expo)

## License

[MIT](LICENSE)
