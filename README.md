# react-native-locale-detector


Fork from [react-native-locale-detector](https://github.com/DylanVann/react-native-locale-detector).

Detects the locale of a user's phone.
Based on [react-native-i18n](https://github.com/AlexanderZaytsev/react-native-i18n), but this just exports the device's locale. This isn't particularly useful on it's own and you'll probably want to use it with an i18n library like [i18next](https://github.com/i18next/i18next).

## Installation

```
npm install react-native-locale-detector --save
cd ios && pod install
```

## Usage

```
// Imports.
import {locale, i18nextReactNative} from 'react-native-locale-detector'
import i18next from "i18next";

i18next
  .use(i18nextReactNative)
  .init();

// We could log it. Maybe it's en-US...
console.log(locale)

// Or if you're using a localization library.
yourLocalizationLibrary.setLocale(locale)
```
