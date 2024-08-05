# RN 0.75 Android Autolinking bug reproduction

This repository reproduces a bug on React Native 0.75 RC where selectively disabling autolinking of a dependency for Android only causes build failures:

```
Project with path ':react-native-vector-icons' could not be found in project ':app'.
```

Where the `react-native-vector-icons` dependency should never even have been part of the generated build config.
