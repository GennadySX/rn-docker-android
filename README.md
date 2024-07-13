# React Native Docker Android CI/CD

This is a simple example of how to use Docker to build a React Native Android app in a CI/CD pipeline.

## Prerequisites

- Docker
- React Native project

## Usage

1. Clone this repository
2. Copy your React Native project into the cloned repository
3. Change 30th line in Docker if your runner in macos or linux
4. Run the following command to build the Docker image:

```bash
docker build -t rn-android-ci .
```

5. Run the following command to build the Android app:

```bash
docker run -v $(pwd)/<your-react-native-project>:/app rn-android-ci
```

6. The Android app will be built in the `android/app/build/outputs/apk/debug` directory
7. You can now use the generated APK file to distribute your app
8. You can also modify the `Dockerfile` to build a release version of the app
9. You can also modify the `Dockerfile` to run tests before building the app
10. You can also modify the `Dockerfile` to deploy the app to a device or emulator
11. You can also modify the `Dockerfile` to deploy the app to the Google Play Store




### License 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

MIT License



### Enjoy!
[![Twitter Follow](https://img.shields.io/twitter/follow/gennadysx.svg?style=social)](https://twitter.com/gennadysx)
![GitHub followers](https://img.shields.io/github/followers/gennadysx.svg?style=social&label=Follow)


Made with ❤️ by Gennady Sabirovsky.
