# RN-Music-Player

A simple and beautiful music player built with React Native, utilizing the [React-Native-Track-Player](https://react-native-track-player.js.org) library for seamless audio playback.

## Features

- **Audio Playback**: Play, pause, skip to next/previous tracks, and seek within songs.
- **Song List**: Displays a list of songs with album art, title, and artist.
- **Progress Slider**: Interactive slider to seek through the current track.
- **Background Playback**: Supports playback controls from the notification bar and lock screen.
- **Responsive UI**: Clean, dark-themed interface optimized for mobile devices.

<!-- ## Screenshots -->

<!-- ![App Screenshot](https://user-images.githubusercontent.com/23727670/118244689-746c3800-b4bd-11eb-98e1-c94acbddd632.png) -->

<!-- ## Demo Video -->

<!-- [![Youtube video](http://img.youtube.com/vi/Ur5-n_D4q5A/maxresdefault.jpg)](http://www.youtube.com/watch?v=Ur5-n_D4q5A) -->

## Download

<a href='https://play.google.com/store/apps/details?id=com.rnmusic.player'><img alt='Get it on Google Play' width="300" src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png'/></a>

# How to run ?

```sh
git clone https://github.com/chayansahu3/Music-Player-React-Native.git

# install node modules
yarn install

# run in android
yarn android

# run in iOS
cd ios && pod install && cd ..
yarn ios

```

## API Integration

This app integrates with the Saavn API for music data.

- **Base URL**: https://saavn.sumit.co/
- **API Key**: Not required
- **Documentation**: [https://saavn.sumit.co/docs](https://saavn.sumit.co/docs)

## Tech Stack

- **React Native** (Expo) with TypeScript
- **React Native Navigation** v6+ (do not use Expo Router)
- **State Management**: Zustand or Redux Toolkit
- **Storage**: MMKV or AsyncStorage
- **Audio Library**: React-Native-Track-Player

## Project Structure

```
RN-Music-Player/
├── android/                 # Android-specific files
├── ios/                     # iOS-specific files
├── src/                     # Source code
│   ├── Controller.js        # Playback controls component
│   ├── data.js              # Sample song data
│   ├── PlayerScreen.js      # Main player screen
│   └── SliderComp.js        # Progress slider component
├── assets/                  # Static assets (album arts, fonts)
├── App.js                   # Main app component
├── index.js                 # App entry point
├── service.js               # Track player service
├── package.json             # Dependencies and scripts
└── README.md                # This file
```

## Setup and Installation

### Prerequisites

- Node.js (v14 or later)
- Yarn or npm
- React Native development environment set up for Android/iOS

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/chayansahu3/Music-Player-React-Native.git
   cd RN-Music-Player
   ```

2. Install dependencies:
   ```sh
   yarn install
   ```

3. For iOS, install CocoaPods dependencies:
   ```sh
   cd ios && pod install && cd ..
   ```

### Running the App

- **Android**:
  ```sh
  yarn android
  ```

- **iOS**:
  ```sh
  yarn ios
  ```

- **Start Metro bundler**:
  ```sh
  yarn start
  ```

## Key Components

- **App.js**: Root component that renders the PlayerScreen.
- **PlayerScreen.js**: Main screen displaying the song list, current track info, and controls.
- **Controller.js**: Handles play/pause, next/previous track buttons.
- **SliderComp.js**: Seek bar for track progress.
- **data.js**: Array of sample songs with metadata and URLs.
- **service.js**: Background service for track player events.

## Dependencies

- `react-native-track-player`: For audio playback functionality
- `@react-native-community/slider`: For the progress slider
- `react-native-vector-icons`: For UI icons
- `react-native-swift`: Additional native modules

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

<!-- ## Related Projects

Check out [@saa27's Music player](https://github.com/saa27/Sangeet) which has additional features. -->

## License

This project is open-source. Please check the license file for details.
