# Star Tracker App (c137)

An Expo/React Native app that lists stars with their distance from Earth and shows detailed star info fetched from a local Flask API.

## Features
- Home screen with a list of stars (name + distance from Earth)
- Details screen showing star distance, gravity, mass, and radius
- Fetches data from a local REST API (`http://127.0.0.1:5000`)
- Stack navigation between Home and Details

## Tech Stack
- React Native 0.64 (Expo SDK 44)
- react-navigation (stack navigator)
- axios
- react-native-elements (Card UI)

## Project Structure
```
c137/
├── App.js                 # entry point + stack navigator
├── package.json
├── app.json
├── babel.config.js
├── assets/                # app icons and splash
└── screens/
    ├── home.js            # star list screen
    └── details.js         # star detail screen
```

## Installation
```bash
npm install
```

## Usage
Start the companion API (serving `/` and `/star?name=...`) on port 5000, then:
```bash
npm start          # or: npm run android / ios / web
```
