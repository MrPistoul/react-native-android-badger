
# react-native-badger-android

## Getting started

`$ npm install react-native-badger-android --save`

### Mostly automatic installation

`$ react-native link react-native-badger-android`

### Manual installation


#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNBadgerAndroidPackage;` to the imports at the top of the file
  - Add `new RNBadgerAndroidPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-badger-android'
  	project(':react-native-badger-android').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-badger-android/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-badger-android')
  	```


## Usage
```javascript
import RNBadgerAndroid from 'react-native-badger-android';

RNAndroidBadger.setBadge(int)
RNAndroidBadger.removeBadge()

enjoy yourself!
