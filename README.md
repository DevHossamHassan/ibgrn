
# instabug-reactnative

## Getting started

`$ npm install https://github.com/DevHossamHassan/ibgrn --save`

### Mostly automatic installation

`$ react-native link instabug-reactnative`

### Manual installation

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.instabug.reactlibrary.RNInstabugReactnativePackage;` to the imports at the top of the file
  - Add `new RNInstabugReactnativePackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':instabug-reactnative'
  	project(':instabug-reactnative').projectDir = new File(rootProject.projectDir, 	'../node_modules/instabug-reactnative/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':instabug-reactnative')
  	```

## Usage
```javascript
import RNInstabugReactnative from 'instabug-reactnative';

// TODO: What do with the module?
RNInstabugReactnative;
```
  
## License

This software is released under <a href="https://opensource.org/licenses/mit-license.php">MIT License</a>.

© 2016 Instabug. All rights reserved.