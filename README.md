# react-native-leenphone

Make SIP calls from react-native using Linphone SDK

## Installation

```sh
npm install react-native-leenphone
```

### IOS

1.
    in `ios/Podfile`add:
    ```rb
    pod 'linphone-sdk', :podspec => '../node_modules/react-native-leenphone/third_party_podspecs/linphone-sdk.podspec'
    pod 'react-native-leenphone', :path => '../node_modules/react-native-leenphone'
    ```
2.
    ```shell
    cd ios && pod install
    ```

### Android
1.
    in `android/app/build.gradle` add:
    ```gradle
    repositories {
      maven {
        url "https://linphone.org/maven_repository"
      }
    }

    dependencies {
      ...
      implementation 'org.linphone:linphone-sdk-android:5.2.110'
    }
   ```
2.
    in `android/build` modify minSdkVersion to 23:
    ```gradle
    buildscript {
       ext {
          ...
          minSdkVersion = 23
          ...
       }
    }
    ```
## Usage



## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the repository and the development workflow.

## License

MIT
