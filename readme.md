# React Native + Expo CNG (Managed Workflow) + Swift iOS Widget Boilerplate

This boilerplate is aimed to demonstrate a bare minimum example of how to implement iOS Widgets with React Native on Expo CNG (Managed Workflow). Notice that `ios` directory is not required. Based on [bndkt/react\-native\-widget\-extension](https://github.com/bndkt/react-native-widget-extension).

## Requirements

Tested under the following environment:

| Software / Library | Version          | Installation Method            |
| ------------------ | ---------------- | ------------------------------ |
| macOS              | 13.5.1 (Ventura) | \* Apple M2 Chip               |
| Node.js            | 18.19.0          | `nodenv`                       |
| EAS CLI            | 7.3.0            | `npm install --global eas-cli` |
| Xcode              | 15.2 (15C500b)   | App Store                      |
| fastlane           | 2.219.0          | `gem install fastlane`         |
| Expo               | 50.0.7           | `create-expo-app`              |
| React Native       | 0.73.4           | `create-expo-app`              |

## Build

```sh
npm install
eas login
eas build:configure
eas build --profile development --platform ios --local
```

## Testing on Simulator

1. `gunzip` the build.
2. Drag & drop the `.app` file into a booted **iPad** simulator. iPhone simulators are known to have issues with widget testing.
3. Add the widget from `Edit Home Screen` menu.
